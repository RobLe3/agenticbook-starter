# Stats Script — Manuscript Measurement Reference

> **Verified:** February 2026 (repo tag v0.6.0)
>
> The stats script measures what a quality-scoring pass cannot: word count trends,
> key-term frequency, and chapter distribution. Run it before and after every revision pass.
> If a "thematic coherence" pass targeting a specific term does not increase that term's
> frequency, the pass did not achieve its stated goal.

---

## Minimal Stats Script

Save as `stats.sh` in your project root. Run with `bash stats.sh` from the project directory.

```bash
#!/bin/bash
# stats.sh — Run from project root
echo "=== Manuscript Statistics ==="
echo ""

echo "Total word count:"
wc -w manuscript/chapters/*.tex 2>/dev/null || wc -w manuscript/*.md 2>/dev/null | tail -1
echo ""

echo "Per-chapter word counts:"
# For LaTeX projects:
for f in manuscript/chapters/ch*.tex; do
  [ -f "$f" ] || continue
  ch=$(basename "$f" .tex)
  cnt=$(wc -w < "$f")
  printf "  %-8s %6d words\n" "$ch:" "$cnt"
done
# For Markdown projects:
for f in manuscript/ch*.md; do
  [ -f "$f" ] || continue
  ch=$(basename "$f" .md)
  cnt=$(wc -w < "$f")
  printf "  %-8s %6d words\n" "$ch:" "$cnt"
done
echo ""

echo "Key term frequency:"
TERMS=("world model" "agent" "verification" "flavor")
for t in "${TERMS[@]}"; do
  # LaTeX:
  cnt=$(grep -ri "$t" manuscript/chapters/*.tex 2>/dev/null | wc -l)
  # Markdown (add if using .md source):
  cnt_md=$(grep -ri "$t" manuscript/*.md 2>/dev/null | wc -l)
  total=$((cnt + cnt_md))
  printf "  %-20s %d occurrences\n" "'$t':" "$total"
done
```

Make executable: `chmod +x stats.sh`

---

## Customizing for Your Project

**Replace the TERMS array** with your book's key terms:

```bash
# Example for a night sky photography book:
TERMS=("exposure triangle" "ISO" "aperture" "dark sky" "light pollution" "Milky Way")

# Example for a business book:
TERMS=("value proposition" "customer" "revenue" "process" "strategy")
```

The adapted TERMS array is your project's intellectual signature — the vocabulary your book is built around. Commit the adapted script alongside your world model.

---

## Extended Stats Script

For more detailed measurement, including chapter-vs-target comparison:

```bash
#!/bin/bash
# stats_extended.sh — Run from project root

# Configure these for your project:
declare -A TARGETS=(
  ["ch01"]=3000
  ["ch02"]=3000
  ["ch03"]=2500
  ["ch04"]=2500
  ["ch05"]=3000
  ["ch06"]=2500
  ["ch07"]=3000
)
KEY_TERMS=("term1" "term2" "term3")  # Replace with your key terms

echo "=== Manuscript Statistics — Extended ==="
echo ""

TOTAL=0
echo "Chapter | Words | Target | Status"
echo "--------|-------|--------|-------"

for f in manuscript/chapters/ch*.tex manuscript/*.md; do
  [ -f "$f" ] || continue
  ch=$(basename "${f%.*}")
  cnt=$(wc -w < "$f")
  TOTAL=$((TOTAL + cnt))
  target=${TARGETS[$ch]:-"—"}
  if [ "$target" = "—" ]; then
    status="—"
  elif [ "$cnt" -ge "$target" ]; then
    status="✓"
  else
    pct=$((cnt * 100 / target))
    status="${pct}%"
  fi
  printf "%-8s  %6d  %6s  %s\n" "$ch" "$cnt" "$target" "$status"
done

echo ""
echo "Total: $TOTAL words"
echo ""

echo "Key term frequency:"
for t in "${KEY_TERMS[@]}"; do
  cnt=$(grep -ri "$t" manuscript/chapters/*.tex manuscript/*.md 2>/dev/null | wc -l)
  printf "  %-25s %d occurrences\n" "'$t':" "$cnt"
done
```

---

## When to Run the Stats Script

| Timing | What to check |
|--------|--------------|
| Before any revision pass | Baseline — word count and term frequency before changes |
| After any revision pass | Delta — what changed? Did the pass achieve its stated goal? |
| Before each milestone commit | Confirm chapters are within target range |
| Before release | Final count; verify nothing is drastically over/under target |

---

## Interpreting the Output

| Observation | What it means |
|-------------|--------------|
| Key term frequency unchanged after a "thematic pass" | The pass targeted quality metrics, not actual vocabulary — reconsider what the pass was supposed to do |
| Chapter consistently 30%+ over target | Chapter scope exceeds its stated intent — consider splitting or cutting |
| Chapter at 50% of target | Chapter may be a stub that needs expansion, or the target is too high for this chapter's content |
| Total word count growing with no revision delta | Content is being added without removing lower-quality material — apply the DO_DONT circuit breaker |
