# Contributing

This guide applies to every eurus-labs repository that has no `CONTRIBUTING.md` of its own. A repository's
`README.md` and `AGENTS.md` add the rules specific to it, such as how to build and test.

## Before you start

- For a small fix, open a pull request directly.
- For anything larger (a new feature, a changed behavior, a refactor across files), open an issue first
  so the approach can be agreed before you spend time on it.
- To report a vulnerability, do not open an issue: follow [SECURITY.md](SECURITY.md).

## Branches

Name branches `<type>/<area>-<outcome>` in lowercase kebab-case, where `<type>` is one of `feat`, `fix`,
`docs`, `refactor`, `test`, `build`, `ci` or `chore`. The name says what the branch changes, for example
`fix/history-dangling-lanes`. Avoid vague words, bare ticket numbers and dates.

## Commits

- Follow [Conventional Commits 1.0.0](https://www.conventionalcommits.org/en/v1.0.0/): a lowercase type
  and optional scope, then an imperative subject of at most 72 characters with no trailing period, for
  example `fix(review): keep findings after a reload`.
- Use the body, wrapped at 72 columns, to explain why the change is needed.
- Mark a breaking change with both `!` after the type and a `BREAKING CHANGE:` footer.
- Commit with your GitHub no-reply address (`<id>+<login>@users.noreply.github.com`), not a private
  email: these repositories are public.
- You are the author of what you submit, whatever tools helped you write it. Do not add AI or tool
  attribution: no tool `Co-Authored-By` trailers, session links or "Generated with" footers.

## Pull requests

- Keep each pull request to one change, based on the latest default branch.
- Fill in the pull request template: why, what changed, the decisions you made, and how you validated it.
- Add tests for features and bug fixes, including the failure case, and run the repository's checks
  before you push.
- If the repository has a `CHANGELOG.md`, add a user-facing entry under the upcoming version.
- CI must pass before review. A maintainer reviews and merges.
