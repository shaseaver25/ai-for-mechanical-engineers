# Session Log: learning-graph-generator v1.07

**Date:** 2026-10-07
**Book:** AI for Mechanical Engineers
**Agent:** Claude Code (Opus 5.5)

## Python programs used

| Program | Version |
|---|---|
| csv-to-json.py | 1.05 (the skill text references 1.04+) |
| analyze-graph.py | not versioned in source |
| taxonomy-distribution.py | not versioned in source |
| validate-learning-graph.py | not versioned in source |

## Steps

1. **Course description assessment**: skipped. `docs/course-description.md` already had
   `quality_score: 100` from course-description-analyzer v0.04, run in the same session.
2. **Concept list**: 306 concepts written to `concept-list.md`. No duplicates and no labels
   over 32 characters. The author reviewed and approved the list as written.
3. **Dependency graph**: `learning-graph.csv` with 453 edges.
4. **Quality validation**: valid DAG, 0 cycles, 0 self-dependencies, 0 orphans,
   8 foundational concepts, 95 terminal nodes (31%), average 1.52 dependencies
   per concept, maximum chain length 20.
   - Fix applied: removed `Learning From Human Feedback (187)` as a prerequisite of
     `AI Chatbot (195)`. It forced RLHF ahead of basic prompting and stretched the
     longest chain from 23 to 20.
   - Gotcha: Python's `csv.writer` defaults to `\r\n` line endings, so a later
     `sed` edit anchored on `$` silently matched nothing. The file was rewritten with
     `lineterminator='\n'`.
5. **Taxonomy**: 13 categories in `concept-taxonomy.md`. Largest is ML at 15.4%,
   smallest is VERIF at 4.2%. None is over 30%.
6. **Taxonomy names, colors, metadata**: `taxonomy-names.json`, `color-config.json`,
   `metadata.json`.
7. **JSON**: `learning-graph.json` (306 nodes, 453 edges, 13 groups). Passed schema
   validation. Top concepts by CIS are Algorithm, Artificial Intelligence,
   Machine Learning, Deep Learning, and Python, all foundational, which confirms the edge direction.
8. **Taxonomy distribution**: `taxonomy-distribution.md`.
9. **Index**: `index.md` from the template. Fixed the "Vew" typo and the "10 entry
   points" placeholder, and added blank lines before links that followed lists.
10. **Nav**: the four generated pages were added under Learning Graph in `mkdocs.yml`.
    `mkdocs build --strict` passes.

## Graph quality score: 85/100

Strengths: clean DAG, balanced taxonomy, sensible foundations, correct edge
direction. Deductions: average in-degree is low (1.52), and Python fundamentals
form fairly linear chains (Variable → Data Type → Integer, and so on).
