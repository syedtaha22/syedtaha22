# Working Rules

These rules apply to every project and to every kind of output: code, documentation, commit
messages and chat. They should be followed without being restated in the work itself.

## 1. Collaboration

### Quality bar

Never deliver the bare minimum. The target is the best possible work: rigor, completeness and
reproducibility. This is not a toy project.

### Questions and edits

A question from the user is a request for an answer, and only that.

- Answer the question. Do not treat it as a request for an edit, or as a signal that something
  was done wrong.
- Edit only when the user explicitly asks for an edit.
- When something the user says is unclear, ask and clarify instead of guessing. Good
  collaboration depends on questions and answers going both ways.

### Scope of the user's own instructions

The user's instructions, preferences and working rules belong in this file and nowhere else.

- Do not write them into project files (README, CONTRIBUTING, docs, templates, code comments,
  docstrings, commit messages). Apply them silently in the work.
- Project files should contain only content about the project itself. They should not contain
  anything invented that the user did not ask for, such as made-up phases or processes.

## 2. Writing Style

These rules cover docs, READMEs, comments, docstrings, commit messages and chat.

### Characters

Never use the em dash (U+2014) anywhere. Use a period, comma, colon, parentheses or a plain " - "
as the sentence needs.

### Modality

State rules, guidelines and expectations with deontic modality ("should", "should not"), not with
indicative statements that use absolutes ("is never", "is always"). For example, write "Tests
should pass before merging", not "Tests are always passing before merging". Statements that
describe how something actually works can stay indicative.

### Qualifiers

Do not describe a prescribed process or rule with qualifiers such as "typical", "usual" or
"normal". State the process as the process.

### Tense and history

Reference only the present state of the project, in files and in chat. Anything stale, absent or
removed (deleted files, renamed items, dropped options, earlier versions, things that were moved
or replaced) should not be mentioned. What is gone is gone.

## 3. Formatting

These rules apply to everything written, whatever the language or file type. The goal is that
a file can be read top to bottom without effort.

### Structure

- Separate logical blocks with a blank line. Do not pack unrelated things together.
- Put one statement, one entry or one item on each line. Expand a collection instead of packing
  it into a single long line, unless it is short enough to read at a glance.
- Keep related items visually grouped and unrelated items visually apart.

### Layout

- Use spaces for indentation, with one consistent width per language, following that language's
  convention. Indent nested content under its parent.
- Keep lines to 100 characters or fewer. Wrap long text at a natural break.
- Remove trailing whitespace and end every file with a single newline.

### Tooling

- Use the formatter that belongs to the language and follow its output instead of formatting by
  hand against it.
- Generated files should meet the same standard as hand-written ones, and should be reformatted
  if the generator packs its output together.

## 4. Code

### Docstrings

- The opening `"""` goes on its own line, the text starts on the next line, and the closing
  `"""` goes on its own line. No text shares a line with the opening `"""`.
- A docstring describes only the code it is attached to: its behaviour, parameters and return
  value. It should not describe external repositories, licences, other files, or anything else
  about the project that is not that code.

### Maintenance burden

Do not add fields, flags, options or states that someone has to remember to maintain later (for
example a status flag that is meant to be set once something is checked). Add only what the
current work uses.

## 5. Git

### Committing

Never commit without the user's explicit permission. Approval for one commit does not extend to
later commits.

### Commit messages

A commit message follows the 50/72 rule: a summary line of 50 characters or fewer, a blank line,
then one paragraph of description wrapped at 72 characters per line.

- It describes only the difference between the previous commit and the new one, as another
  developer sees it in the diff. To write one, inspect the actual diff against the last commit.
- It should not mention how the changes came about: intermediate steps, mistakes, fixes made
  along the way, or anything that does not exist in the diff.
- It should not contain a Co-Authored-By trailer or any other attribution line.
