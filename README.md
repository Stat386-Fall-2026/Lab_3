# Lab 3: Exploring Data with pandas

In this lab, you will use pandas to explore a dataset of General Conference
talks. You will practice inspecting a DataFrame, filtering observations,
sorting values, calculating summary statistics, grouping data, and creating a
new variable. You will present your work in a rendered Quarto document.

## Create your personal repository

1. Click **Use this template** and select **Create a new repository**.
2. For **Owner**, select `Stat386-Fall-2026`.
3. Name your repository using the format `your_netid_lab_3`.
4. Set the repository visibility to **Private**.
5. Click **Create repository**.

## Clone and set up the project

Clone your personal repository inside your `School/STAT_386` folder:

```bash
git clone <your-repository-url>
cd <your-repository-name>
```

Install the project dependencies:

```bash
uv sync
```

The first time you run this command, `uv` will also create a `uv.lock` file.
Include that file in your first commit.

Open the repository folder in Positron. If Positron asks you to select a Python
interpreter, select the interpreter inside the `.venv` folder created by `uv`.

## Complete the lab

Open `lab_3.qmd` and replace `Your Name` with your name. Complete every code
section and every written response. You can preview the document while you
work by running:

```bash
uv run quarto preview lab_3.qmd
```

Stop the preview by pressing `Ctrl+C` in the terminal.

Make several meaningful commits as you work. For example:

```bash
git add lab_3.qmd
git commit -m "Complete data inspection and filtering"
git push
```

## Render and submit

Before submitting, restart your work from a clean session and render the final
document:

```bash
uv run quarto render lab_3.qmd
```

Commit and push both the source document and the rendered HTML file:

```bash
git add lab_3.qmd lab_3.html
git commit -m "Complete Lab 3"
git push
```

Follow the submission directions provided in Canvas.

## Generate the Follow-Up Reflection Issue

Create a new Issue using the **Lab 3 Complete** Issue template if it is available.

Use the following information:

**Title**

```text
Lab 3 complete
```
The description of this issue can be empty.

Post the Lab 3 processing command in a new comment:

```text
@local-llm-user process config-dir: Lab_3/ in instructor-repo: Stat386-Fall-2026/Instructor_Repo
```

Again, the command must be posted as a **comment**, not in the Issue description.

The collaborator should create a new job. Once processing is complete, the course collaborator should create a new Issue containing review questions for Lab 3.

Answer the questions as a comment in the newly created issue to finish the lab.

## Before you finish

- [ ] Your name appears in the document header.
- [ ] Every code section is complete.
- [ ] Every written response is complete.
- [ ] `lab_3.qmd` renders without errors.
- [ ] `lab_3.html` is committed to the repository.
- [ ] `uv.lock` is committed to the repository.
- [ ] All commits are pushed to GitHub.

## Repository contents

```text
Lab_3/
├── data/
│   └── talks.csv
├── .gitignore
├── README.md
├── lab_3.qmd
└── pyproject.toml
```

The `uv.lock` file will be added when the project environment is first
synchronized.
