# Contributing to LLazyEmail

Conventions shared across the organization. Individual repositories may add more specific rules in their own `CONTRIBUTING.md` and `AGENTS.md`.

## Principles

1. **Small, single-purpose draft PRs** — one concern each; stack when needed; wait for CI.
2. **Extend, do not delete** curated content — restructure, annotate, or move to `archive/` instead of wholesale removal.
3. **Do not merge or close PRs** unless the human owner explicitly asks.
4. **Never invent stats** (stars, download counts, versions). Cite GitHub / npm / the repository itself.
5. **Never commit secrets** (tokens, passwords, private keys). Use `secrets: inherit` on reusable workflow calls only when required.

## Commit trailer

When working for the maintainer (Arthur Tkachenko / atherdon / petroved), every commit includes:

```text
Co-authored-by: petroved <arthur.tkachenko.netweight@gmail.com>
```

## AGENTS.md for AI agents

Most active repositories ship an [`AGENTS.md`](https://github.com/search?q=org%3ALLazyEmail+filename%3AAGENTS.md&type=code) at the repo root. Agents should:

1. Read `AGENTS.md` before changing behavior.
2. Treat `src/` (and tests) as ground truth; docs explain intent.
3. Prefer injected `render` functions into `@llazyemail/generate-template` over local reimplementations of catalog / payload / write.
4. Prefer thin callers of [`documentation-actions@v1`](https://github.com/LLazyEmail/documentation-actions) and [`email-template-workflows@v1`](https://github.com/LLazyEmail/email-template-workflows) instead of copying job YAML.
5. Pin third-party Actions to a **full commit SHA** with a `# vX.Y.Z` comment; Renovate keeps them current.
6. Open **draft** PRs against `main` unless told otherwise.

Useful agent entry points:

| Repo | Guide |
| --- | --- |
| [generate-template](https://github.com/LLazyEmail/generate-template/blob/main/AGENTS.md) | Catalog / `run` / CLI contracts |
| [markup-generator](https://github.com/LLazyEmail/markup-generator/blob/main/AGENTS.md) | Monorepo packages + npm publish |
| [template-runtime-display](https://github.com/LLazyEmail/template-runtime-display/blob/main/AGENTS.md) | Inspector + email shell |
| [email-template-workflows](https://github.com/LLazyEmail/email-template-workflows/blob/main/AGENTS.md) | Action modes + gotchas |
| [documentation-actions](https://github.com/LLazyEmail/documentation-actions/blob/main/AGENTS.md) | Docs CI adoption |
| [hn_email_template](https://github.com/LLazyEmail/hn_email_template/blob/main/AGENTS.md) | Current generator vs legacy archive |
| [documentation](https://github.com/LLazyEmail/documentation/blob/main/AGENTS.md) | Docs site layout |

Also see `llms.txt` / `llms-full.txt` in several repos (for example email-template-workflows, template-runtime-display, markdown-regex).

## Shared CI / workflow conventions

### Email rendering — `email-template-workflows`

Pin `LLazyEmail/email-template-workflows@v1` (floating major). Modes:

- **command** — e.g. `npx generate-template --all --out=generated`
- **script** — npm script with input/output flags
- **build-command** — MJML / pandoc / arbitrary CLI once per template

Uploads a browsable artifact, writes a job summary, and can upsert a PR comment. Examples live under that repository’s `examples/`.

### Documentation — `documentation-actions`

Pin `LLazyEmail/documentation-actions@v1` after release (draft adoption may use `@main` only during the adoption window). Provides:

- Reusable workflows: Docusaurus test-deploy / Pages deploy, docs-ci umbrella, link check (lychee), markdownlint, changelog, docs-index, catalog-api, auto-rebase, star-request, awesome-list checks
- Composite actions under `actions/<name>/`
- Skill checklist: [`skills/docusaurus-docs-site/SKILL.md`](https://github.com/LLazyEmail/documentation-actions/blob/main/skills/docusaurus-docs-site/SKILL.md)

The actions index is **append-only** (`docs/actions-index.md` in that repo): new actions add one table row at the end.

## Changelog and release flow

Patterns vary by package type; do not hand-edit compiled changelogs when a fragment system exists.

### `.changelog/` fragments (Actions / workflows repos)

Used by `email-template-workflows` and `documentation-actions`:

1. PR adds a flat file under `.changelog/` (`semver:` required; optional `type:`).
2. CI validates fragments (`skip-changelog` / `no-changelog` labels waive).
3. A release workflow folds fragments into `CHANGELOG.md` and opens `rel/vX.Y.Z`.
4. Merging the release PR (or tagging) publishes a GitHub Release; floating major tags (`v1`) move on publish.

### Changesets (library packages)

Used by `generate-template` and similar:

1. `npx changeset` for user-facing changes.
2. Version Packages PR updates `CHANGELOG.md` and versions.
3. Publishing happens when a GitHub Release is published (or via the package’s `npm-publish` / `publish` workflow).

### Public npm vs GitHub Packages

| Registry | Examples |
| --- | --- |
| **npmjs.com** (public) | `markup-generator`, `markdown-regex`, `@lazyemail/markdown-to-email`, `email-template-object` |
| **GitHub Packages** (`npm.pkg.github.com`, scope `@llazyemail`) | `@llazyemail/generate-template`, `@llazyemail/render-template`, `@llazyemail/template-runtime-display`, `@llazyemail/validator`, `@llazyemail/simple-tags` (package name `simple-tags`) |

Install GitHub Packages with a token that has `read:packages` and an `.npmrc` that maps `@llazyemail` — see each repo’s `.npmrc.example`.

`markup-generator` publishes to the **public npm registry** with trusted publishing / OIDC (`id-token: write`); internal `@llazyemail/*` workspace packages are **bundled** into the published tarball in v4.x.

## Code of collaboration

- Prefer draft PRs; request review when CI is green.
- Align Docusaurus sites (config shape, tokens, search, SEO, footer) across documentation / awesome lists / v-school / assemblya.
- For awesome lists: never delete curated entries wholesale; fix links, annotate dead ones, or extend sections.
