# Gemini CLI playground

This file is intended to be the single source of truth for all the Gemini CLI
related information.

## Prompts

This section should contain the most important prompts that have been used to
build this project.

## Markdown style

Markdown files within this project, with no exceptions, must follow well-defined
and straightforward guidelines for their style.
These are defined in the file `.markdownlint.json` within the root directory.
As of today (2025-09-10), the file specifies the following rules:

* **MD003 - Heading style**: This rule is triggered when different heading
  styles are used within the same document. The purpose of this rule is to
  enforce consistency in your Markdown files, which makes them easier to read
  and understand. In this project, the `atx` style is enforced, which means
  using `#` for all heading levels.

* **MD013 - Line length**: This rule checks for line length and flags any line
  longer than 80 characters. This is to ensure readability. Code blocks are
  excluded from this rule.

* **MD040 - Fenced code blocks should have a language specified**: This rule is
  disabled in this project.

To check whether a document adheres to the guidelines, if
[markdownlint-cli2](https://github.com/DavidAnson/markdownlint-cli2) is
installed, you can run it with the following command.

```shell
markdownlint-cli2 --config .markdownlint.json <FILE>
```

Where `<FILE>` is the filename you want to check.

In case of errors, you will have an output similar to the following.

```shell
gilberto@margot playground-gemini-cli % markdownlint-cli2 --config .markdownlint.json GEMINI.md
markdownlint-cli2 v0.18.1 (markdownlint v0.38.0)
Finding: GEMINI.md
Linting: 1 file(s)
Summary: 2 error(s)
GEMINI.md:22 MD012/no-multiple-blanks Multiple consecutive blank lines [Expected: 1; Actual: 2]
GEMINI.md:23 MD012/no-multiple-blanks Multiple consecutive blank lines [Expected: 1; Actual: 3]
```

The errors show the violated rule (e.g., `MD012`) and the line where it is
violated (e.g., line 22 in `GEMINI.md`).
You can use this information to fix the problem.

## References

* [Gemini CLI Tutorial Series](https://medium.com/google-cloud/gemini-cli-tutorial-series-77da7d494718)
