# .github

Organization-wide defaults for [eurus-labs](https://github.com/eurus-labs).

| File | What GitHub does with it |
| ---- | ------------------------ |
| [`profile/README.md`](profile/README.md) | Shows it on the organization's profile page. |
| [`CONTRIBUTING.md`](CONTRIBUTING.md) | Links it from new issues and pull requests in every repository without its own. |
| [`SECURITY.md`](SECURITY.md) | Uses it as the security policy of every repository without its own. |
| [`.github/ISSUE_TEMPLATE/`](.github/ISSUE_TEMPLATE/) | Offers these issue forms in every repository without its own `ISSUE_TEMPLATE` folder. |
| [`.github/pull_request_template.md`](.github/pull_request_template.md) | Pre-fills new pull requests in every repository without its own template. |
| [`.github/workflows/commits.yml`](.github/workflows/commits.yml) | Reusable check that repositories call: Conventional Commits, no AI or tool attribution, GitHub no-reply identities. Tag releases `v1`, `v1.1.0`… |
| [`renovate-config.json`](renovate-config.json) | Shared Renovate preset: opens a pull request in each repository when Template publishes a new tag (`"extends": ["github>eurus-labs/.github:renovate-config"]`). |

A repository's own file always wins: these defaults only fill gaps. Skills, for example, has its own
`CONTRIBUTING.md`, so the one here does not apply there.

Agent instructions are not inherited from this repository. Repositories get the shared rules from
[Template](https://github.com/eurus-labs/Template) through Copier, and Renovate keeps them current.
