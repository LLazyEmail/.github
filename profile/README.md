# LLazyEmail 👋

Tools, templates and React components for building emails: write in Markdown, get responsive HTML or React email templates out.

📖 **Documentation:** [llazyemail.github.io/documentation](https://llazyemail.github.io/documentation/) · [Source on GitHub](https://github.com/LLazyEmail/documentation)

## Quick navigation

| I want to... | Go to |
| :--- | :--- |
| Convert Markdown to email | [Main project](#-main-project) |
| Browse every repository | [Repository index](#-repository-index) |
| Use React email components | [React design system](#-react-design-system) |
| Start a new template | [Starters & templates](#-starters--templates) |
| Learn how it all works | [Learning resources](#-learning-resources) |
| See similar projects | [Related projects](#-related-projects) |

---

## 🚀 Main project

**[markdown-to-email](https://github.com/LLazyEmail/markdown-to-email)** is the core engine. It parses Markdown and renders responsive HTML or React email templates.

![Mind map of the markdown-to-email project](https://github.com/atherdon/markdown-to-email/blob/main/MindMap1.png?raw=true)

**Where to look in the code**

- [Content source](https://github.com/LLazyEmail/markdown-to-email/blob/main/src/domain/content-source/index.js)
- [Replace Markdown (HTML)](https://github.com/LLazyEmail/markdown-to-email/blob/main/src/domain/replace-markdown/html/replace-md.js)
- [Replace Markdown (React)](https://github.com/LLazyEmail/markdown-to-email/blob/main/src/domain/replace-markdown/react/replace-md.js)
- [Write module](https://github.com/LLazyEmail/markdown-to-email/tree/main/src/domain/write)

<details>
<summary><b>npm modules used by markdown-to-email</b></summary>

```
"atherdon-callbacks": "^1.10.0",
"atherdon-newsletter-html-replacer": "^0.4.0",
"atherdon-newsletter-js-layouts": "^1.5.1",
"atherdon-newsletter-react": "^1.0.11",
"atherdon-newsletter-react-replacer": "^0.4.0",
"atherdon-old-newsletter-js-outertemplate": "^2.4.0",
"markup-generator": "^0.4.0",
```

</details>

---

## 🗂 Repository index

### Core engine and utilities

| Repository | Description |
| :--- | :--- |
| [markdown-to-email](https://github.com/LLazyEmail/markdown-to-email) | Core engine for transforming Markdown into responsive HTML/React email templates |
| [markup-generator](https://github.com/LLazyEmail/markup-generator) | File output and markup-writing generator utility |
| [generator-markdown-to-html](https://github.com/LLazyEmail/generator-markdown-to-html) | Generator module for Markdown to HTML |
| [markdown-regex](https://github.com/LLazyEmail/markdown-regex) | Regex constants for parsing Markdown syntax |
| [template-object](https://github.com/LLazyEmail/template-object) | Factory object for display classes, helps manage email template displays |
| [amazon-ses-service](https://github.com/LLazyEmail/amazon-ses-service) | AWS SES sending integration |

### ⚛️ React design system

| Repository | Description |
| :--- | :--- |
| [react-email-template](https://github.com/LLazyEmail/react-email-template) | Core React components for structural email layouts (the "React One" template) |
| [react-email-table](https://github.com/LLazyEmail/react-email-table) | Cross-client HTML table wrappers for React emails |
| [react-email-typography-components](https://github.com/LLazyEmail/react-email-typography-components) | Components for structured email typography |
| [react-email-miscellaneous-components](https://github.com/LLazyEmail/react-email-miscellaneous-components) | Miscellaneous React helpers for email layouts |
| [react-email-letter-components](https://github.com/LLazyEmail/react-email-letter-components) | Letter-style components for email creation |
| [react-sendgrid-form](https://github.com/LLazyEmail/react-sendgrid-form) | Form component integration for SendGrid |
| [email-template-react](https://github.com/LLazyEmail/email-template-react) | React email template |
| [nextjs-preview](https://github.com/LLazyEmail/nextjs-preview) | Next.js preview app for templates |

### 🧱 Starters & templates

| Repository | Description |
| :--- | :--- |
| [default-email-template](https://github.com/LLazyEmail/default-email-template) | General email boilerplate, good for cloning |
| [generator-module](https://github.com/LLazyEmail/generator-module) | Example generator module for cloning |
| [replacer](https://github.com/LLazyEmail/replacer) | Example replacer module for cloning |
| [pixel-email-cli](https://github.com/LLazyEmail/pixel-email-cli) | Example CLI for cloning |
| [template-typography](https://github.com/LLazyEmail/template-typography) | Starter for custom email typography packages |
| [free-email-templates-to-try](https://github.com/LLazyEmail/free-email-templates-to-try) | Free, ready-to-use HTML email templates |
| [react-plain-template-example](https://github.com/LLazyEmail/react-plain-template-example) | Plain JavaScript and React DOM template example |
| [remix-ecommerce-react-email-template](https://github.com/LLazyEmail/remix-ecommerce-react-email-template) | E-commerce email starter built with React |

### 🟨 Plain JS templates

| Repository | Description |
| :--- | :--- |
| [hn_email_template](https://github.com/LLazyEmail/hn_email_template) | HN template |
| [mjml-email-template](https://github.com/LLazyEmail/mjml-email-template) | MJML version |
| [nomoretogo_email_template](https://github.com/LLazyEmail/nomoretogo_email_template) | NMTG version |
| [_trying-lit](https://github.com/LLazyEmail/_trying-lit) | Plain JS template (`atherdon-old-newsletter-js-outertemplate`) |

### 🧪 Experimental and curated

| Repository | Description |
| :--- | :--- |
| [_trying_simple_tags](https://github.com/LLazyEmail/_trying_simple_tags) | Sandbox for HTML/tag parsing |
| [awesome-email-marketing](https://github.com/LLazyEmail/awesome-email-marketing) | Curated list of email marketing tools, articles and frameworks |

---

## 📚 Learning resources

### Must read

- [Build your email templates with React](https://medium.com/ovrsea/build-your-email-templates-with-react-ea530ba6b010)
- [Creating email templates with React components](https://assertible.com/blog/creating-email-templates-with-react-components)
- [HTML Email Basics](https://templates.mailchimp.com/getting-started/html-email-basics/)
- [How to build emails with React](https://building.lang.ai/how-to-build-emails-with-react-fcf941b125d1)
- [Build a Reusable Design System With React](https://code.tutsplus.com/tutorials/build-a-reusable-design-system-with-react--cms-29954)
- [Create elegant HTML email templates using React](https://bestofreactjs.com/repo/chromakode-react-html-email-react-renderers)
- [React-email-editor](https://github.com/unlayer/react-email-editor)

### Articles by Arthur Tkachenko

<details>
<summary><b>Building templates and components</b></summary>

- [Organizing an Advanced Structure for HTML Email Template](https://hackernoon.com/organizing-an-advanced-structure-for-html-email-template)
- [How I Started to Build React Components for Email Templates](https://hackernoon.com/how-i-started-to-build-react-components-for-email-templates)
- [Introducing a Simple NPM Module with Email Templates](https://hackernoon.com/introducing-a-simple-npm-module-with-email-templates)
- [Building a Design System for Email Templates (React)](https://hackernoon.com/building-a-design-system-for-email-templates-react)

</details>

<details>
<summary><b>Email marketing and strategy</b></summary>

- [5 Reasons Why Newsletters Should Be Part Of Your Business Strategy](https://hackernoon.com/5-reasons-why-newsletters-should-be-part-of-your-business-strategy)
- [Email Marketing and How to Curate an Effective Business Newsletter](https://hackernoon.com/email-marketing-and-how-to-curate-an-effective-business-newsletter)
- [Exploring Substack for Building Your Newsletter](https://hackernoon.com/exploring-substack-for-building-your-newsletter)
- [Businesses Have Messy Emails](https://hackernoon.com/businesses-have-messy-emails)
- [Businesses Have Messy Emails: The Relationship between Security and Sales](https://hackernoon.com/businesses-have-messy-emails-the-relationship-between-security-and-sales)

</details>

<details>
<summary><b>Tools, lists and glossary</b></summary>

- [Glossary for Non Technies](https://hackernoon.com/glossary-for-non-technies)
- [#Together4Victory: List of Email Marketing Tools](https://hackernoon.com/together4victory-list-of-email-marketing-tools)
- [Cool Newsletters for developers [Part 1]](https://hackernoon.com/cool-newsletters-for-developers-part-1)
- [Cool resources for sending emails](https://hackernoon.com/cool-resources-for-sending-emails)

</details>

### Logging and tooling

- [Designing Error Messages and a Logging Strategy in Node.js](https://blog.appsignal.com/2021/11/03/designing-error-messages-and-a-logging-strategy-in-nodejs.html)
- [Comparing Node.js logging tools](https://blog.logrocket.com/comparing-node-js-logging-tools/)
- [npmlog](https://www.npmjs.com/package/npmlog)
- [How to use levels function in Logger](https://www.tabnine.com/code/javascript/functions/npmlog/Logger/levels)
- [How to handle log events with the npmlog library?](https://stackoverflow.com/questions/72506435/how-to-handle-log-events-with-the-npmlog-library)
- [markdownlint](https://www.npmjs.com/package/markdownlint)
- [Mintlify docs](https://www.mintlify.com/docs)

---

## 🔭 Related projects

Worth a look for ideas and comparison:

- [Bojler](https://github.com/Slicejack/bojler)
- [Maizzle](https://github.com/maizzle/maizzle)
- [Pechkin](https://github.com/sglazov/pechkin)
- [11ty-email-generator](https://github.com/5t3ph/11ty-email-generator/blob/main/src/_data/meta.js)
