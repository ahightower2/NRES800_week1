# Assignment 01: The Reproducibility "Hello World"

**Due:** Sunday, Aug 30, 11:59 PM

## Why am I doing this?

Setting up a reproducible workflow is the most important step in modern data
science. This assignment connects your "home base" (RStudio Project) to your
"communication line" (GitHub). By finishing it you prove you can move from raw
data to a rendered report and share it — the foundation for everything else this
semester.

## What do I need to do?

1. **Accept the assignment** from the GitHub Classroom link and clone your repo.
2. **Open `assignment.qmd`** and fill in every `TODO` and blank (`___`).
3. In the setup chunk: load `tidyverse` and `here`, then load penguins with
   `data(penguins, package = "palmerpenguins")`.
4. Build a scatterplot of **bill length** vs **bill depth**, colored by
   **species**. Save it to the object `penguin_plot` (already named for you).
5. Write the provenance note, a 2-sentence interpretation, and the AI methods note.
6. **Render** to HTML (the "Render" button, or `quarto render assignment.qmd`).
7. **Edit this README** — This project utilizes a standard R package called palmerpenguins to practice analyze and visualize data through coding. Primary commands used are library(), data(), ggplot(), aes(), geom_point(), and labs(). The final product is a scatterplot showing bill length and depth color coded by the three species.
8. **Commit and push** everything (source `.qmd` and rendered `.html`).

## What do I submit?

Push your repository. It must contain:

- `assignment.qmd` and the rendered `assignment.html`
- This `README.md`, completed
- The automated checks (a green checkmark, or a red X you have read and understood)

## How will I be graded?

See `rubric.md` in this repo. Short version: reproducibility (renders on a clean
clone), organization (`here()`, no absolute paths), communication (a specific
interpretation and a complete README), and version control (everything pushed).

## The automated feedback bot

When you push, a GitHub Action renders your document and runs checks. A red X is
not a grade — it means the robot found something to look at. Click the check to
read the log, fix, and push again. This is the real professional loop: push →
read the log → fix → repush.

## Where can I get help?

- **Errors:** post a screenshot to GitHub Discussions.
- **Concepts:** ask a neighbor or the instructor at the next Debug Clinic.
- **AI policy:** you may use AI to troubleshoot errors. Document it in the
  Methods Note at the bottom of `assignment.qmd`.
