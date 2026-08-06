# MVP — Minimum Bar

This is done when all of the following are true:

- [ ] **Column data types.** At least **5 of 6** columns have a correct
  inferred data type, each with a one-sentence reason based on what you
  actually saw running the `cut` command for that column in `field_notes.md`
  — not a guess from the column name alone, and not a type you can't
  actually point to a real value for.
- [ ] **List vs. table.** In your own words, you explain the actual
  difference between a list/array and a table.
- [ ] **Structured vs. unstructured.** You state which one this dataset is,
  and why.
- [ ] **Two collection-process concerns.** At least 2 specific things you'd
  want to know about how this dataset was collected before trusting it.
- [ ] **One data-quality question.** The most checkable of those 2 concerns,
  turned into a real question for the source — specific and answerable, not a
  generic "is this data good?" A good test: could the data's maintainer
  actually answer it with a yes/no or a specific fact?
- [ ] **A separate curiosity question.** Something *you* genuinely want to
  explore with this data — not the same question as the data-quality one.
- [ ] **AI-literacy reflection.** 2 concrete risks of trusting unverified AI
  output about this data, plus one specific, checkable personal rule for
  double-checking an AI-provided fact.
- [ ] **Terminal log.** `field_notes.md`'s "Setup log" section and section 9
  filled in as you actually worked — real commands in fenced ` ```bash `
  blocks, including one real error and how you diagnosed it from the message.
- [ ] **GitHub repo.** Public, contains `field_notes.md` and a `README.md`.
  No Python file is expected — this project doesn't test writing code.
- [ ] **Commit history.** At least **2 commits**, each with a real, descriptive
  message (`add raw data`, `add column-type notes`, etc.) — not one
  everything-at-once commit and not messages like `update` or `final`.

That's the whole bar — more than it looks at first glance, but every item is
a short, honest reflection or a real command you already had to run, not new
code to write.
