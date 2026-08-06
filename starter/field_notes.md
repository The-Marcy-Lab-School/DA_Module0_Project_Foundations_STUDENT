# Data Literacy Field Notes

Dataset: `../data/co2_emissions_2022.csv` (see `../data/SOURCE.md`). Every
section below gives you the exact terminal command to run — paste the
**real output** you got, then write your answer based on what you actually
saw, not what you'd expect. Work through this in order; open the raw file
before anything else.

Run all commands from the repo root, or `cd` into `data/` first and drop the
`data/` prefix — your choice, just be consistent.

## 1. First look at the raw file

Before anything else, look at the file as plain text — don't jump to
inspecting it column-by-column yet.

```bash
head -4 data/co2_emissions_2022.csv
```

**Output:**
```
_TODO: paste what you actually got_
```

**What I notice:** _TODO — your raw observations, in your own words_

## 2. Column names

```bash
head -1 data/co2_emissions_2022.csv | tr ',' '\n'
```

**Output:**
```
_TODO_
```

## 3. Column-by-column data type table

For each column, preview real values with `cut` (change `-f` to the column's
number: `country`=1, `iso_code`=2, `year`=3, `population`=4, `gdp`=5,
`co2`=6). Example for `country`:

```bash
cut -d, -f1 data/co2_emissions_2022.csv | head -6
```

Run the equivalent for at least 5 of the 6 columns, then fill in the table
from what you actually saw — not a guess from the column name alone:

| Column | Inferred type | How I can tell |
|---|---|---|
| _TODO_ | _TODO_ | _TODO_ |
| _TODO_ | _TODO_ | _TODO_ |
| _TODO_ | _TODO_ | _TODO_ |
| _TODO_ | _TODO_ | _TODO_ |
| _TODO_ | _TODO_ | _TODO_ |

**In your own words:** what's the actual difference between a list/array
and a table? (Not a definition you looked up — explain it the way you'd
explain it to a friend who's never coded. No command needed for this one,
just think about the table you just filled in above.)

_TODO_

## 4. Structured or unstructured?

State which this dataset is, and why.

_TODO_

## 5. Before you trust this data

List **at least 2** specific things you'd want to know about how this
dataset was collected, before trusting any conclusion drawn from it. Ground
at least one in something you actually checked — try these:

```bash
tail -n +2 data/co2_emissions_2022.csv | cut -d, -f2 | grep -c '^$'
```
(Counts how many rows have a **blank** `iso_code`. `tail -n +2` skips the
header, `cut -d, -f2` pulls just that column, `grep -c '^$'` counts empty
lines.)

**Output:**
```
_TODO_
```

```bash
tail -n +2 data/co2_emissions_2022.csv | cut -d, -f5 | grep -c '^$'
```
(Same idea, for the `gdp` column.)

**Output:**
```
_TODO_
```

**My 2 concerns:**
1. _TODO_
2. _TODO_

## 6. Data-quality question for the source

Take the **most specific and checkable** of the two concerns above, and
phrase it as a real question you'd send to the data's source/maintainer. A
good test: could they actually answer it with a concrete yes/no or fact —
not "is this data good?"

_TODO_

## 7. Something you're actually curious about

Different question from #6 — that one was about checking the data's
trustworthiness. This one's about you: what's something you're genuinely
curious to explore using this data? Look up a specific row or two to help
form the question — e.g.:

```bash
grep "^China," data/co2_emissions_2022.csv
grep "^India," data/co2_emissions_2022.csv
```

(Swap in any two countries you're actually curious to compare.)

**Output:**
```
_TODO_
```

**My question:** _TODO_

## 8. AI-literacy reflection

Name **2 concrete risks** of trusting an AI assistant's output about this
dataset (or any data question) without checking it yourself. Then state
**one specific personal rule** for when you'll double-check an AI-provided
fact before relying on it professionally — specific enough that you could
actually follow it, not "I'll be careful."

**Risks:**
1. _TODO_
2. _TODO_

**My rule:** _TODO_
