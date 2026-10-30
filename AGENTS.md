# Repository Guidelines

## Project Structure & Module Organization

SadBoard is a planning-stage embedded Linux troubleshooting project for QEMU and physical development boards. Only documentation exists; scenarios and CLI commands are not implemented.

- `README.md`: scope, implementation status, and documentation index.
- `docs/bootlin-linux-debugging-guide.md`: Chinese Bootlin study guide and proposed SadBoard exercises.
- `AGENTS.md`: contributor and agent instructions.

There are no source, test, or asset directories. Add learning guides under `docs/` and link them from `README.md`. Keep proposed features distinct from working functionality.

## Build, Test, and Development Commands

No build system, dependencies, server, or automated tests are configured. For documentation changes, run:

- `git diff --check`: check tracked changes for whitespace errors.
- `git diff -- AGENTS.md README.md docs/`: review tracked documentation edits.
- `git status --short`: identify modified and untracked files.

Untracked files do not appear in ordinary diffs; inspect them directly. Once staged, use `git diff --cached --check` and `git diff --cached`. Bootlin lab commands are external instructions, not SadBoard build targets.

## Coding Style & Naming Conventions

Write learning guides in Chinese; preserve official tool names, identifiers, and commands. Use descriptive Markdown headings, `-` lists, backticks for paths, and language-tagged code fences. Indent nested lists consistently with spaces.

Use lowercase, hyphen-separated guide filenames, such as `linux-memory-debugging-guide.md`. No formatter, linter, or language-specific configuration exists.

## Validation and Scenario Guidelines

Check heading structure, relative links, source citations, and platform assumptions. Preview Markdown when available and report any unverified rendering. No test framework or coverage threshold exists.

For proposed exercises, describe symptoms, prerequisites, trigger conditions, expected evidence, root cause, repair verification, and reset procedure. Record architecture, kernel version, configuration, and required tools. Distinguish reviewed instructions from reproduced results; report where commands actually ran.

## Commit & Pull Request Guidelines

Follow the existing `docs: <imperative summary>` convention; keep commits focused. PRs should describe affected documents, purpose, validation, and related issues. Include screenshots only when useful for rendering changes.

Preserve unrelated work. The project is SadBoard, while its configured remote is `linux-bsp/BadBoard`; do not rename either implicitly.

## Sources & Attribution

Preserve Bootlin links and CC BY-SA 3.0 attribution for adapted material. Label original project proposals separately from official course content. No project code license has been selected.
