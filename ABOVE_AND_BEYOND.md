# Above & Beyond

Finished the MVP with time to spare? Each of these previews a skill a later
module assumes you already have — pick one or two, don't feel obligated to do
all of them. None of these require writing code — Module 0 doesn't test
that — except the last one, which explicitly gives you the code to run.

- **Chain terminal commands to answer a real question about the dataset that
  a single command couldn't.** Pipe (`|`) or sequence (`&&`) 2-3 commands —
  `grep`, `head`, `wc`, `cut`, whatever fits — to find something real (row
  count, how many rows match a pattern, whatever you're curious about). A
  starting idea: of the rows missing `gdp` (section 5), how many are real
  countries (non-empty `iso_code`) vs. aggregate rows? That needs an `awk`
  one-liner combining both conditions — worth looking up. Log the chain and
  what it told you in `field_notes.md`. This is the same terminal fluency
  **Module 7, 8, and 9's** heavier data-engineering/pipeline work assumes you
  already have.

- **Find the min and max of a numeric column** — `sort -n` a column
  numerically, then `head -1`/`tail -1` for the min/max:
  ```bash
  tail -n +2 data/co2_emissions_2022.csv | cut -d, -f6 | grep -v '^$' | sort -n | head -1
  tail -n +2 data/co2_emissions_2022.csv | cut -d, -f6 | grep -v '^$' | sort -n | tail -1
  ```
  (that's the `co2` column — try `population` or `gdp` too). You're not doing
  real exploratory data analysis yet (that's **Module 2**), but noticing "this
  range looks suspicious" or "this min is exactly 0 — is that a true zero or
  a missing-value placeholder?" is the same instinct EDA is built on.

- **Practice deciding whether to approve an AI-suggested command — the way
  you will constantly once you're using tools like Claude Code for real.**
  Ask an AI assistant for a terminal command to do something in this project
  (clean up a file, check disk usage, whatever's genuinely useful). **Before
  running it:** explain in your own words exactly what the command does, and
  specifically flag anything destructive or hard to undo — `rm`/`rm -rf`,
  `git reset --hard`, a force-push, anything that deletes or overwrites
  without asking again. Then decide: approve it as-is, modify it, or reject
  it — and say why. Only then actually run whatever you approved, and log the
  real result in `field_notes.md`. This is `ai-literacy` and
  `terminal-command-line` at the same time, and it's exactly the judgment
  call **Module 4** (Python for Data Analysis, your first real
  AI-assisted-coding work) and **Module 13** (Generative/Agentic AI Tooling)
  assume you already practice by instinct — a command an AI suggests is a
  *suggestion*, not something to run just because it was suggested.

- **Use a branch instead of committing straight to `main`.** Create a branch
  for your field-notes work, commit there, then merge it back. Real git
  workflows (which come back in force in **Module 4**'s project work and
  again in **Module 8**'s pipeline/orchestration work and the **Module 15**
  capstone) rarely involve committing straight to `main`.

- **Preview of Module 1 — code given, you don't need to write this
  yourself.** Everything above used terminal commands; Module 1 is where you
  start writing this kind of logic yourself in Python. Here's a tiny, real
  taste of it — a function that does roughly the same type-guessing you did
  by eye in section 3, but in code. Save this as `preview.py` and run it
  (`python3 preview.py`) if you have Python installed; if not, just read
  through it:
  ```python
  def guess_type(value):
      """Given one value (as a string), guess what type of data it is."""
      if value == "":
          return "missing"
      try:
          int(value)
          return "whole number"
      except ValueError:
          pass
      try:
          float(value)
          return "decimal number"
      except ValueError:
          pass
      return "text"

  print(guess_type("40578847"))    # a population value
  print(guess_type("10.170"))      # a co2 value
  print(guess_type("Afghanistan")) # a country name
  print(guess_type(""))            # a missing gdp value
  ```
  In `field_notes.md`, write 1-2 sentences comparing this to what you did by
  hand: does `guess_type()` agree with your own column-type table from
  section 3? Where might it disagree, and why?

None of these change what counts as "done" per `MVP.md` — they're optional,
and a complete MVP without any of these is still a full, passing submission.
