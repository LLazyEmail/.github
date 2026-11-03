# LLazyEmail repository catalog

Inventory of **public** repositories under [`LLazyEmail`](https://github.com/LLazyEmail), generated from `gh repo list` metadata and each repository’s README. Star counts and archive flags are taken from the GitHub API at documentation time — do not invent stats.

- Public repos listed: **74**
- Archived: **3**
- Forks: **4**

See also: [architecture](./architecture.md) · [contributing](./contributing.md) · [profile README](../profile/README.md)

## Core pipeline

| Repository | Description | Language | ★ |
| --- | --- | --- | ---: |
| [markup-generator](https://github.com/LLazyEmail/markup-generator) | module for writing content into files | TypeScript | 0 | |
| [generate-template](https://github.com/LLazyEmail/generate-template) | Configurable engine for rendering named email templates to HTML (@llazyemail/generate-template) | TypeScript | 0 | |
| [render-template](https://github.com/LLazyEmail/render-template) | Deterministic HTML part/compose renderer with traces (@llazyemail/render-template) | TypeScript | 0 | |
| [template-runtime-display](https://github.com/LLazyEmail/template-runtime-display) | Email shell + runtime + inspector on top of render-template | TypeScript | 0 | |
| [email-template-workflows](https://github.com/LLazyEmail/email-template-workflows) | Reusable GitHub Action that installs your project's dependencies, renders email HTML with whatever you already use (an npm script, MJML, Maizzle, pandoc, a catalog CLI), uploads a browsable artifact, writes a job summary, and on a pull request posts or updates one comment. | Shell | 0 | |
| [validator](https://github.com/LLazyEmail/validator) | Small TypeScript validation helpers (@llazyemail/validator) | TypeScript | 0 | |

## Markdown tooling

| Repository | Description | Language | ★ |
| --- | --- | --- | ---: |
| [markdown-to-email](https://github.com/LLazyEmail/markdown-to-email) | Core Markdown → responsive HTML/React email engine | JavaScript | 8 | |
| [markdown-regex](https://github.com/LLazyEmail/markdown-regex) | Set of constants that can help you to parse markdown content | TypeScript | 10 | |
| [generator-markdown-to-html](https://github.com/LLazyEmail/generator-markdown-to-html) | Markdown → HTML via unified/remark/rehype (GFM by default) | TypeScript | 1 | |
| [markdown-to-email-demo](https://github.com/LLazyEmail/markdown-to-email-demo) | Demo repository showing markdown-to-email in action | JavaScript | 1 | |

## Production templates

| Repository | Description | Language | ★ |
| --- | --- | --- | ---: |
| [hn_email_template](https://github.com/LLazyEmail/hn_email_template) | Plain-JS Hackernoon-style newsletter generator using template-runtime-display | JavaScript | 1 | |
| [nomoretogo_email_template](https://github.com/LLazyEmail/nomoretogo_email_template) | NoMoreToGo / MailerLite-style email template monorepo (active work under template/) | HTML | 1 | |
| [postmark-transactional-template-simple](https://github.com/LLazyEmail/postmark-transactional-template-simple) | Standalone transactional email template generator (Postmark-oriented) | TypeScript | 0 | |
| [_playing_with_lit](https://github.com/LLazyEmail/_playing_with_lit) | Lit SSR experiments converting HTML email templates; consumer of generate-template | HTML | 0 | |

## Documentation & curated lists

| Repository | Description | Language | ★ |
| --- | --- | --- | ---: |
| [documentation](https://github.com/LLazyEmail/documentation) | Primary LLazyEmail Docusaurus documentation site (docs.llazyemail.com) | HTML | 0 | |
| [documentation-actions](https://github.com/LLazyEmail/documentation-actions) | Reusable GitHub Actions and workflows for Docusaurus and awesome-list repos | Shell | 0 | |
| [awesome-email-marketing](https://github.com/LLazyEmail/awesome-email-marketing) | ✉️ An awesome list of resources for email marketing. | TypeScript | 78 | |
| [awesome-newsletters](https://github.com/LLazyEmail/awesome-newsletters) | Curated newsletter directories, articles, tools, and craft resources | JavaScript | 4 | |
| [v-school](https://github.com/LLazyEmail/v-school) | Docusaurus docs for v-school (inventory, 3D parts, printing, lectures; EN + UK) | JavaScript | 0 | |
| [assemblya](https://github.com/LLazyEmail/assemblya) | Docusaurus docs site for AssemBLYA (EN + UK); working fork of atherdon/assemblya | HTML | 0 | · fork |
| [fuck-ecoflow](https://github.com/LLazyEmail/fuck-ecoflow) | Docusaurus documentation site (working fork of atherdon/fuck-ecoflow; Git LFS media) | JavaScript | 0 | · fork |

## React design system

| Repository | Description | Language | ★ |
| --- | --- | --- | ---: |
| [react-email-template](https://github.com/LLazyEmail/react-email-template) | Core React structural email layout components ("React One") | JavaScript | 0 | |
| [react-email-table](https://github.com/LLazyEmail/react-email-table) | Cross-client HTML table wrappers for React emails | JavaScript | 0 | |
| [react-email-typography-components](https://github.com/LLazyEmail/react-email-typography-components) | Typography components for React emails | JavaScript | 0 | |
| [react-email-miscellaneous-components](https://github.com/LLazyEmail/react-email-miscellaneous-components) | Miscellaneous React helpers for email layouts | JavaScript | 0 | |
| [react-email-letter-components](https://github.com/LLazyEmail/react-email-letter-components) | Letter-style React components for emails | HTML | 0 | |
| [react-sendgrid-form](https://github.com/LLazyEmail/react-sendgrid-form) | SendGrid form component integration | JavaScript | 1 | |
| [email-template-react](https://github.com/LLazyEmail/email-template-react) | This template will be a simple way to clone and use folders for different new templates | JavaScript | 0 | |
| [nextjs-preview](https://github.com/LLazyEmail/nextjs-preview) | Next.js preview app for email templates | JavaScript | 2 | |
| [react-plain-template-example](https://github.com/LLazyEmail/react-plain-template-example) | Plain JS + React DOM template example (architecture similar to Lit / NMTG repos) | JavaScript | 0 | |

## Remix / brand starters

| Repository | Description | Language | ★ |
| --- | --- | --- | ---: |
| [remix-ecommerce-react-email-template](https://github.com/LLazyEmail/remix-ecommerce-react-email-template) | Remix starter: ecommerce email (React design system) | JavaScript | 0 | |
| [remix-hn-react-email-template](https://github.com/LLazyEmail/remix-hn-react-email-template) | Remix starter: Hackernoon-style React email | JavaScript | 0 | |
| [remix-amazon-billing-email-template](https://github.com/LLazyEmail/remix-amazon-billing-email-template) | Remix starter: Amazon-style billing email (React design system) | JavaScript | 0 | |
| [remix-google-billing-email-template](https://github.com/LLazyEmail/remix-google-billing-email-template) | Remix starter: Google-style billing email | JavaScript | 0 | |
| [remix-stripe-billing-email-template](https://github.com/LLazyEmail/remix-stripe-billing-email-template) | Remix starter: Stripe-style billing email | JavaScript | 0 | |
| [remix-taskrabbit-react-email-template](https://github.com/LLazyEmail/remix-taskrabbit-react-email-template) | Remix starter: TaskRabbit-style React email | JavaScript | 0 | |
| [remix-uber-react-email-template](https://github.com/LLazyEmail/remix-uber-react-email-template) | Remix starter: Uber-style React email | JavaScript | 0 | |
| [remix-venmo-react-email-template](https://github.com/LLazyEmail/remix-venmo-react-email-template) | Remix starter: Venmo-style React email | JavaScript | 0 | |
| [template-react-email-template](https://github.com/LLazyEmail/template-react-email-template) | Template repository for React email design-system starters | JavaScript | 0 | |
| [js-remix-google-template](https://github.com/LLazyEmail/js-remix-google-template) | Google-style billing email remix starter | — | 0 | |

## Starters, editors & utilities

| Repository | Description | Language | ★ |
| --- | --- | --- | ---: |
| [default-email-template](https://github.com/LLazyEmail/default-email-template) | General email boilerplate intended for cloning | JavaScript | 4 | |
| [free-email-templates-to-try](https://github.com/LLazyEmail/free-email-templates-to-try) | Free ready-to-use HTML email templates collection | HTML | 2 | |
| [pixel-email-cli](https://github.com/LLazyEmail/pixel-email-cli) | Example CLI for email generation (cloneable) | JavaScript | 0 | |
| [template-typography](https://github.com/LLazyEmail/template-typography) | template repository for creating typography package | JavaScript | 1 | |
| [template-object](https://github.com/LLazyEmail/template-object) | Factory/object helpers for email template display classes (npm email-template-object) | JavaScript | 0 | |
| [typography-typed](https://github.com/LLazyEmail/typography-typed) | Prop and function types for shared email components | TypeScript | 0 | |
| [email-file-size](https://github.com/LLazyEmail/email-file-size) | The weight of the HTML is important because Gmail clips messages that weigh over 102kb | TypeScript | 0 | |
| [amazon-ses-service](https://github.com/LLazyEmail/amazon-ses-service) | AWS SES sending integration helpers | JavaScript | 10 | |
| [mjml-email-template](https://github.com/LLazyEmail/mjml-email-template) | MJML-based email template experiments | HTML | 0 | |
| [email-template-editor](https://github.com/LLazyEmail/email-template-editor) | Early email template editor experiments | JavaScript | 0 | |
| [email-template-editor-nodejs](https://github.com/LLazyEmail/email-template-editor-nodejs) | Node.js email template editor experiments | HTML | 1 | |
| [email-template-editor-reactjs](https://github.com/LLazyEmail/email-template-editor-reactjs) | Visual editor for HTML emails as a tree of blocks (React) | TypeScript | 1 | |
| [nmtg-email-editor](https://github.com/LLazyEmail/nmtg-email-editor) | NoMoreToGo email editor experiments | HTML | 0 | |
| [subscribe-form](https://github.com/LLazyEmail/subscribe-form) | Subscription form front-end / server launcher | JavaScript | 0 | |
| [subscription-server](https://github.com/LLazyEmail/subscription-server) | Node.js subscription API (MongoDB) | JavaScript | 0 | |

## Experiments & sandboxes

| Repository | Description | Language | ★ |
| --- | --- | --- | ---: |
| [_trying_simple_tags](https://github.com/LLazyEmail/_trying_simple_tags) | Plain JS typography helpers: tiny pure functions that turn props into HTML strings | TypeScript | 0 | |
| [_trying-oclif](https://github.com/LLazyEmail/_trying-oclif) | Standalone oclif CLI experiment for the LLazyEmail rendering engine | TypeScript | 0 | |
| [templates-battlefield](https://github.com/LLazyEmail/templates-battlefield) | Sandbox / battlefield for template experiments | JavaScript | 0 | |
| [content-marketing](https://github.com/LLazyEmail/content-marketing) | Hub for planning, drafting, scheduling, and tracking LLazyEmail content | DIGITAL Command Language | 0 | |
| [creative](https://github.com/LLazyEmail/creative) | Creative / design scratch repository | HTML | 1 | |
| [copy-vouchful](https://github.com/LLazyEmail/copy-vouchful) | Vouchful-related copy / content experiments | HTML | 0 | |
| [emayla](https://github.com/LLazyEmail/emayla) | Email-рассылка related experiments | HTML | 0 | |
| [gh](https://github.com/LLazyEmail/gh) | Markdown archive / tooling related to GrowthHackingIdea newsletter emails | Python | 0 | |
| [tkachenko-articles](https://github.com/LLazyEmail/tkachenko-articles) | Index of Arthur Tkachenko articles related to email / newsletters | — | 0 | |
| [website](https://github.com/LLazyEmail/website) | Legacy / marketing website content | CSS | 0 | |
| [tasks](https://github.com/LLazyEmail/tasks) | Task tracking scratch repository | — | 0 | |
| [demo-repository](https://github.com/LLazyEmail/demo-repository) | A code repository designed to show the best GitHub has to offer. | HTML | 0 | |
| [mjml-showcase](https://github.com/LLazyEmail/mjml-showcase) | MJML showcase / samples | — | 0 | |

## Forks

| Repository | Description | Language | ★ |
| --- | --- | --- | ---: |
| [oy](https://github.com/LLazyEmail/oy) | Render HTML emails on the server with React. | JavaScript | 0 | · fork |
| [lit-element-starter-js](https://github.com/LLazyEmail/lit-element-starter-js) | Sample component project using LitElement, in JavaScript | JavaScript | 0 | · fork |

## Other active repositories

| Repository | Description | Language | ★ |
| --- | --- | --- | ---: |
| [.github](https://github.com/LLazyEmail/.github) | Organization profile README and shared org meta for github.com/LLazyEmail | — | 0 | |

## Archived / legacy

GitHub-archived repositories (collapsed for the profile README). Prefer current packages above.

| Repository | Description | Language | ★ |
| --- | --- | --- | ---: |
| [_trying_frontmatter](https://github.com/LLazyEmail/_trying_frontmatter) | Archived front-matter parsing experiments | JavaScript | 0 | · **archived** |
| [lit-typography](https://github.com/LLazyEmail/lit-typography) | Archived lit-typography package experiments | JavaScript | 0 | · **archived** |
| [replacer](https://github.com/LLazyEmail/replacer) | Replacer module finally getting a separated place | JavaScript | 0 | · **archived** |

## Notes

- Historical profile links such as `generator-module` and `_trying-lit` are **not** present in the current public org inventory (they may have been renamed or removed).
- `replacer`, `lit-typography`, and `_trying_frontmatter` are **archived** on GitHub.
- Star counts (`★`) come from the GitHub API and change over time.
