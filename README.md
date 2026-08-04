# Foundations Project: Data Literacy Field Notes

**New here?** Start with `GETTING_STARTED.md` — it walks through turning this
template into your own repo.

**Due:** 2 days (this first project is intentionally short — a couple of
focused days right after this module's content phase, not a full week, since
it's meant to get you moving, not to be a big lift).

## Skills you'll practice

- **Programming fundamentals** — reasoning about variables, data types, and data structures
- **Data literacy** — inspecting an unfamiliar dataset and describing it accurately
- **Git & version control** — real, incremental commit history
- **AI literacy** — distinguishing a verified fact from an unverified AI claim
- **Curiosity** — asking a real, specific question you want to explore in data
- **Critical thinking** — questioning a dataset's collection process, not just its surface
- **Terminal / command line** — navigating and working entirely from the shell

## What you're building

Set up your personal data-analytics development environment, then produce a
**"Data Literacy Field Notes" mini-notebook**: inspect a small, previously-unseen
real public dataset, document each column's inferred data type and whether the
dataset is structured or unstructured, and note one specific data-quality
question you'd ask the data's source. Push the notebook plus a README to a new
**public GitHub repository** with at least two well-messaged commits.

This is the very first project of the program — it isn't testing deep data
skills yet. It's testing whether you can set up a real development workflow
(terminal, git, GitHub) and look at unfamiliar data carefully and honestly,
both habits everything else in this program builds on.

## Dataset

Use **OWID's CO2 and Greenhouse Gas Emissions dataset**:
https://github.com/owid/co2-data (the `owid-co2-data.csv` file in that repo).

License: **CC BY 4.0** — verified directly against the repo's own README
("All visualizations, data, and code produced by *Our World in Data* are
completely open access under the Creative Commons BY license"). You're free to
use it in your public repo; credit Our World in Data as the source.

If you'd rather use a different dataset, World Bank Open Data
(https://data.worldbank.org/) is also cleared — CC BY 4.0, confirmed against
its actual terms-of-use page — but pick one specific indicator/table from it
rather than the whole portal, and keep it small enough to actually read
end-to-end in a couple of days.

Don't substitute a dataset that isn't one of these two without checking its
license yourself first — "small and previously unseen" doesn't mean "whatever
comes up first in a search."

## Setup

Tools for this module (all free): **Terminal** (bash/zsh — pre-installed on
macOS/Linux, or Git Bash/WSL on Windows), **Git**, **GitHub** (free tier —
unlimited public repos), **VS Code**.

See `GETTING_STARTED.md` for turning this template into your own repo and
setting up `.gitignore`/`LICENSE`/your first commit yourself. Once that's
done: download `owid-co2-data.csv` from the dataset link above and you're
ready to start.

## What to do

See `starter/field_notes.ipynb` for the notebook skeleton (fill it in section
by section — don't skip straight to the code cell) and `milestones.md` for a
suggested pace across the 2 days. Your instructor shares the full step-by-step
checklist and grading rubric separately through the classroom — not this repo.
