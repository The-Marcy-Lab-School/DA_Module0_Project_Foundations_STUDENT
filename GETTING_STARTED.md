# Getting Started

This repo is a **GitHub template** — a starting point, not something you edit
directly on Marcy's copy of it. This is the first project of the whole
program, so this doc assumes you've never done any of this before.

## Step 1: Get your own copy

On this repo's GitHub page, you'll see two buttons that both sound like "make
a copy" but do different things:

- **"Use this template"** ← use this one. It creates a brand-new, independent
  repository under *your* GitHub account, with no visible link back to this
  template. That's what you want for something that becomes part of your
  portfolio.
- **"Fork"** — creates a copy that stays linked to this one (GitHub will show
  "forked from marcy-lab-school/..." on your repo forever). Fork is the right
  tool when you intend to contribute changes back to the original project —
  that's not this. Don't use Fork here.

Click **"Use this template" → "Create a new repository,"** name it something
like `data-literacy-field-notes`, keep it **public** (the assignment requires
a public repo), and create it.

## Step 2: Clone your new repo locally

On your own new repo's page (not this template), click the green **Code**
button, copy the HTTPS URL, then in your terminal:

```
git clone <the URL you copied>
cd <your-repo-name>
```

## Step 3: Set up your environment yourself

This module is literally about learning git, GitHub, and the terminal — so
unlike some later projects, this template does **not** come with a
`.gitignore` or a `LICENSE` already made. Building them is part of the
assignment, not busywork:

- **Create a `.gitignore`.** From the terminal: `touch .gitignore`, then open
  it in VS Code and add a few lines for files Python/Jupyter projects
  shouldn't track — think about what actually shouldn't go in version control
  (compiled files, checkpoint files your notebook editor creates
  automatically, OS-generated files like `.DS_Store`). Don't just copy a
  `.gitignore` from somewhere — write the 3-4 lines that apply to *this*
  project, so you understand what each one is for.
- **Choose a `LICENSE`.** Since this repo is going public, add a license so
  it's clear what others can do with your code. MIT is a common, simple
  default for a personal project — see https://choosealicense.com if you want
  to understand the tradeoffs before picking.
- **Make your first commit.** Once you've added those two files:
  ```
  git add .gitignore LICENSE
  git commit -m "add gitignore and license"
  git push
  ```

You should already have `git init`-equivalent setup from cloning (cloning
sets up the local repo and connects the remote for you) — if you're not sure
`git status` and `git remote -v` both work cleanly in this folder, that's the
first thing to check before moving on.

## Step 4: Do the actual project

See `README.md` for the dataset and what you're building, `starter/
field_notes.ipynb` for the notebook skeleton, and `milestones.md` for a
suggested day-by-day pace. Your instructor will separately share the full
checklist and grading rubric through the classroom, not this repo.
