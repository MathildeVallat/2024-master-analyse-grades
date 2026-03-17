# Grade Analysis — Eval Grades

An R/Quarto data analysis project completed during a Master's programme, exploring
student grade data across courses, groups, and semesters.

---

## Overview

This project analyses a dataset of 44,195 grades from 761 students across multiple
courses and groups. The analysis covers grade distributions, course correlations,
final grade calculations, and student pass rates.

---

## Requirements

**R packages:**
```r
install.packages(c("here", "readr", "ggplot2", "dplyr", "tidyr", "scales"))
```

**Data:**

Place `grades.csv` in a `data/` folder in the project root. The file should contain
columns for: `id`, `group`, `course`, `semester`, and `grade`.

---

## Project Structure
```
eval-grades.Rproj
├── data/
│   └── grades.csv
└── subject-17.qmd
```

---

## Analysis Questions

| # | Topic |
|---|-------|
| 1–3 | Load data; count total grades and students |
| 4–5 | Student–group mapping; students per group |
| 6 | Average grades by group for *Art and Expression* |
| 7 | Grade distribution by semester |
| 8 | Summary statistics for grades per student |
| 9–11 | Grade counts in *Combat Tactics and Self-Defense* by group |
| 12–13 | Per-course average grades; scatter plot across courses |
| 14–15 | Correlation between courses by group; most correlated group |
| 16–17 | Final grade calculation; comparison by group |
| 18–19 | Pass/fail logic; students with high grades who still fail |
| 20 | Pass rate per group with visualisation |

---

## Pass/Fail Criteria

A student passes if **both** conditions are met:

- Average grade ≥ **5** in every individual course
- Average grade ≥ **10** in every semester

---

## Output

Rendered as both **HTML** and **PDF** via Quarto (`format: html` and `format: pdf`).

To render:
```bash
quarto render subject-17.qmd
```
