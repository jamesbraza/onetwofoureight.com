# AGENTS.md

## Project Overview

Personal blog/website at <https://onetwofoureight.com>,
built with [Hugo](https://gohugo.io/)
and the [Hermit-V2][1] theme.

[1]: https://github.com/1bl4z3r/hermit-V2

## Tech Stack

- Static site generator: Hugo
- Theme: [Hermit-V2][1]
  - Imported as a Hugo module via `go.mod`
- Config: `hugo.toml`
- Content: Markdown files in `content/`
- Hosted: GitHub Pages
- Deploy: `.github/workflows/hugo.yaml`

## Development

### Building locally

```sh
hugo server
```

### Hugo theme updates

```sh
hugo mod get github.com/1bl4z3r/hermit-V2@<version>
hugo mod tidy
```

When updating, check the [Hermit-V2 releases][3] for breaking changes.

[3]: https://github.com/1bl4z3r/hermit-V2/releases

### Linting

Pre-commit hooks handle all linting. Run manually with:

```sh
prek run --all-files
```

CI runs linting via `prek-action` (see `.github/workflows/lint-test.yaml`).

### Style

- Markdown content uses [semantic linefeeds][2] (one sentence per line)
- Line length limit: 120 chars for prose, 88 for code blocks
  (see `pyproject.toml` configuration of `tool.pymarkdown`)

[2]: https://rhodesmill.org/brandon/2012/one-sentence-per-line
