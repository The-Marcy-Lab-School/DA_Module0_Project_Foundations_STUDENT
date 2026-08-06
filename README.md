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
- **Terminal / command line** — this is the main hands-on skill this project tests. You'll inspect real data entirely from the command line (`head`, `cut`, `grep`, `wc`, `sort`) — no Python required or expected yet, that starts in Module 1.

## What you're building

Set up your personal data-analytics development environment, then produce
**"Data Literacy Field Notes"**: inspect a small, previously-unseen real
public dataset **using terminal commands**, document each column's inferred
data type and whether the dataset is structured or unstructured, note one
specific data-quality question you'd ask the data's source, a separate
question you're personally curious to explore, and a short AI-literacy
reflection. Push it all plus a README to a new **public GitHub repository**
with at least two well-messaged commits.

This is the very first project of the program — it isn't testing deep data
skills yet, and it isn't testing *writing* code (that starts in Module 1;
"Programming fundamentals" above means explaining ideas like data types and
data structures in your own words, not writing a program). It's testing
whether you can set up a real development workflow (terminal, git, GitHub)
and look at unfamiliar data carefully and honestly **using the terminal
commands you already have**, both habits everything else in this program
builds on.

## Dataset

Everyone in this cohort uses the same dataset — already included at
`data/co2_emissions_2022.csv`, no download needed. It's a small, curated
slice (254 rows, 6 columns, the year 2022) of OWID's full public CO2 and
Greenhouse Gas Emissions dataset. See `data/SOURCE.md` for exactly how it
was derived and its license (CC BY 4.0, Our World in Data).

Don't substitute a different dataset — using the same one across the cohort
keeps everyone's grading consistent and means classmates can actually compare
notes on what they found.

## Setup (macOS)

Everyone in this cohort is on macOS, so these directions assume that —
skip anything about other operating systems, you won't need it.

Tools for this module (all free):

- **Terminal** — already on your Mac (Applications → Utilities → Terminal, or
  `Cmd+Space` and type "Terminal").
- **Git** — check if it's already installed: open Terminal and run `git
  --version`. If it's not installed, macOS will prompt you to install the
  Xcode Command Line Tools — accept that prompt.
- **GitHub** — free tier, unlimited public repos. Create an account if you
  don't have one.
- **VS Code** — download from https://code.visualstudio.com (the macOS
  `.dmg` build), drag it into Applications. You'll use it to edit Markdown
  files and open a terminal — not to write or run any code this project.

See `GETTING_STARTED.md` for turning this template into your own repo and
setting up `.gitignore`/`LICENSE`/your first commit yourself.

## What to do

See `starter/field_notes.md` for the field-notes template — every section
tells you which terminal command to run, and you fill in the real output you
got plus your answer. `starter/TERMINAL_LOG.md` is the required running log
of commands you actually use (start filling it in from Step 1, don't
reconstruct it at the end). `milestones.md` has a suggested pace across the
2 days. Your instructor shares the full step-by-step checklist and grading
rubric separately through the classroom — not this repo.
