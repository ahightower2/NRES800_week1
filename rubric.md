# Assignment Rubric — Week 01: The Reproducibility Hello World

## Technical Correctness (4 pts)

- [ ] A `ggplot2` scatterplot of `bill_length_mm` vs `bill_depth_mm` is present and visible in the rendered HTML
- [ ] `color = species` is inside `aes()` (not a fixed color string)
- [ ] `library(tidyverse)` and `library(here)` appear in the setup chunk; `palmerpenguins` data loaded via `data(penguins, package = "palmerpenguins")`
- [ ] No hardcoded paths; `here()` used for any file references

**What "correct" looks like for this assignment:** The rendered HTML contains a colored scatterplot where each species (Adelie, Chinstrap, Gentoo) appears as a distinct color. The plot shows bill length on the x-axis and bill depth on the y-axis. A 2-sentence interpretation follows the plot.

## Reproducibility (3 pts)

- [ ] The `.qmd` file renders to HTML without errors on a clean clone (no manual console steps required)
- [ ] All required packages loaded at the top of the document in a setup chunk
- [ ] Raw data accessed via `data()` call, not from a manually placed CSV
- [ ] README describes what the project contains (2–3 sentences minimum)

## Style & Documentation (3 pts)

- [ ] Variable names: `snake_case`, descriptive
- [ ] Interpretation sentence is specific (describes a visible pattern, not "I made a plot")
- [ ] No unused `library()` calls or orphaned objects in the document
- [ ] AI use note present at end of `.qmd` if AI was used

---

## Grading Notes (Instructor Only)

**Most common failure mode (Week 01):** Document loads packages in console but not in the `.qmd` — renders fine for the student but fails on a clean machine. Check that the setup chunk contains all `library()` calls.

**`color` outside `aes()` error:** `color = "blue"` (fixed color, no mapping) should lose the Technical Correctness point for species color. `color = species` outside `aes()` will throw an error — deduct from Reproducibility as well.

**GitHub check:** Confirm rendered `.html` is present in the repo (not just the `.qmd`). Students who only push source lose the Version Control points.

**Partial credit for interpretation:** Award full Communication credit if the sentence names a direction (longer bills → deeper bills? or bill length and depth are inversely related by species?) even if not perfectly phrased. Penalize only if the sentence is completely generic ("the plot shows data").
