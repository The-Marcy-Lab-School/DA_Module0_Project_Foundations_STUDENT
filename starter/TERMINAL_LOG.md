# Terminal Log

A running record of real commands you actually ran for this project — not
every keystroke, but enough that someone reading this could see how you
actually worked. Add to it as you go, don't reconstruct it from memory at
the end.

**Formatting:** write each command in its own fenced code block tagged
`bash`, like this:

````
```bash
git status
```
````

That's three backticks, the word `bash`, your command(s), then three
backticks to close. It renders with proper syntax highlighting and makes the
command copy-pasteable — this is the standard way to show terminal commands
in any README, docs site, or GitHub issue you'll ever write.

---

## Setup

```bash
# TODO: the commands you actually ran to set up this repo
```

## Working the project

```bash
# TODO: real commands as you go -- cd, ls, git add/commit, running your
# notebook, whatever you actually typed
```

## A command chain (optional but recommended)

Terminal commands can be **chained** — piped into each other with `|`, or
run in sequence with `&&` — so you do in one line what would otherwise take
several separate commands. Example shape (not necessarily useful for this
exact dataset, just showing the pattern):

```bash
head -5 owid-co2-data.csv | tr ',' '\n' | wc -l
```

That pipes the first 5 lines into `tr` (replace commas with newlines) into
`wc -l` (count lines) — a fast, no-Python way to sanity-check how many
columns a row has. If you find a real use for chaining in this project,
log it here.

## An error you hit and how you diagnosed it

```bash
# TODO: paste the actual command and the actual error message
```

_TODO: what did the error message actually tell you, and how did that lead
to the fix — not "I googled it," what specifically changed._
