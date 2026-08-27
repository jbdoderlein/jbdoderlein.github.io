# al-folio

<div align="center">

[![Preview](readme_preview/al-folio-preview.png)](https://alshedivat.github.io/al-folio/)

**A simple, clean, and responsive [Jekyll](https://jekyllrb.com/) starter for academic websites.**

_In `v1.x`, al-folio is a **thin starter, not a theme**: the runtime ships as independently versioned plugin gems, so you pick up fixes and features by bumping a pinned version in your `Gemfile` instead of merging theme internals into your site._

---

[![deploy](https://github.com/alshedivat/al-folio/actions/workflows/deploy.yml/badge.svg)](https://github.com/alshedivat/al-folio/actions/workflows/deploy.yml)
[![Maintainers](https://img.shields.io/badge/maintainers-4-success.svg)](#maintainers)
[![GitHub contributors](https://img.shields.io/github/contributors/alshedivat/al-folio.svg)](https://github.com/alshedivat/al-folio/graphs/contributors/)

[![Docker Image Version](https://img.shields.io/docker/v/amirpourmand/al-folio?sort=semver&label=docker%20image&color=blueviolet)](https://hub.docker.com/r/amirpourmand/al-folio)
[![Docker Image Size](https://img.shields.io/docker/image-size/amirpourmand/al-folio?sort=date&label=docker%20image%20size&color=blueviolet)](https://hub.docker.com/r/amirpourmand/al-folio)
[![Docker Pulls](https://img.shields.io/docker/pulls/amirpourmand/al-folio?color=blueviolet)](https://hub.docker.com/r/amirpourmand/al-folio)

[![GitHub release](https://img.shields.io/github/v/release/alshedivat/al-folio)](https://github.com/alshedivat/al-folio/releases/latest)
[![GitHub license](https://img.shields.io/github/license/alshedivat/al-folio?color=blue)](https://github.com/alshedivat/al-folio/blob/main/LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/alshedivat/al-folio)](https://github.com/alshedivat/al-folio/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/alshedivat/al-folio)](https://github.com/alshedivat/al-folio/fork)

[![Code Wiki](https://img.shields.io/badge/Code_Wiki-ask_about_repo-blue?logo=googlegemini)](https://codewiki.google/github.com/alshedivat/al-folio)
[![DeepWiki](https://img.shields.io/badge/DeepWiki-ask_about_repo-lightcyan)](https://deepwiki.com/alshedivat/al-folio)

</div>

## Getting started

**⚠️ Important: Use "Use this template" (not fork)**

When creating your own website with al-folio, you have two options:

- ✅ **Recommended:** Click "[Use this template](https://github.com/new?template_name=al-folio&template_owner=alshedivat)" – This creates a clean copy that is independent from the main al-folio repository. Changes you make to your site won't be accidentally submitted to al-folio as pull requests.
- ❌ **Not recommended:** Forking the repository – This keeps a link to the main al-folio repo, making it easy to accidentally submit your personal site changes as contributions to our project.

**If you already forked:** Don't worry! You can still work with your fork normally. Just make sure to:

1. Make changes on a dedicated branch (e.g., `my-site-updates`)
2. When pushing changes, always verify you're pushing to **your own repository**, not the main al-folio repository
3. Never create pull requests to `alshedivat/al-folio` unless you're intentionally contributing improvements that benefit all users

For quick setup, see [docs/QUICKSTART.md](docs/QUICKSTART.md).

Want to learn more about Jekyll? Check out [this tutorial](https://www.taniarascia.com/make-a-static-website-with-jekyll/). Why Jekyll? Read [Andrej Karpathy's blog post](https://karpathy.github.io/2014/07/01/switching-to-jekyll/)! Why write a blog? Read [Rachel Thomas blog post](https://medium.com/@racheltho/why-you-yes-you-should-blog-7d2544ac1045).

## Table Of Contents

<!--ts-->

- [al-folio](#al-folio)
  - [Getting started](#getting-started)
  - [Table Of Contents](#table-of-contents)
  - [Installing and Deploying](#installing-and-deploying)
  - [Customizing](#customizing)
  - [Plugin Ecosystem](#plugin-ecosystem)
  - [Using AI Agents](#using-ai-agents)
    - [Codex](#codex)
    - [Claude](#claude)
    - [Copilot And Other Agents](#copilot-and-other-agents)
  - [Documentation](#documentation)
  - [Features](#features)
    - [Light and dark mode](#light-and-dark-mode)
    - [The pages you get out of the box](#the-pages-you-get-out-of-the-box)
    - [Writing](#writing)
    - [GitHub repositories and stats](#github-repositories-and-stats)
  - [User community](#user-community)
  - [Lighthouse PageSpeed Insights](#lighthouse-pagespeed-insights)
    - [Desktop](#desktop)
    - [Mobile](#mobile)
  - [FAQ](#faq)
  - [Contributing](#contributing)
    - [Code quality checks](#code-quality-checks)
    - [Maintainers](#maintainers)
    - [All Contributors](#all-contributors)
  - [Star History](#star-history)
  - [License](#license)
- [al-folio](#al-folio-1)
  - [User community](#user-community-1)
  - [Lighthouse PageSpeed Insights](#lighthouse-pagespeed-insights-1)
    - [Desktop](#desktop-1)
    - [Mobile](#mobile-1)
  - [Table Of Contents](#table-of-contents-1)
  - [Getting started](#getting-started-1)
  - [Installing and Deploying](#installing-and-deploying-1)
  - [Customizing](#customizing-1)
  - [GitHub Copilot Agents](#github-copilot-agents)
    - [Customization Agent](#customization-agent)
    - [Documentation Agent](#documentation-agent)
  - [Documentation](#documentation-1)
  - [Features](#features-1)
    - [Light/Dark Mode](#lightdark-mode)
    - [CV](#cv)
    - [People](#people)
    - [Publications](#publications)
    - [Collections](#collections)
    - [Layouts](#layouts)
      - [The iconic style of Distill](#the-iconic-style-of-distill)
      - [Full support for math &amp; code](#full-support-for-math--code)
      - [Photos, Audio, Video and more](#photos-audio-video-and-more)
    - [Other features](#other-features)
      - [GitHub's repositories and user stats](#githubs-repositories-and-user-stats)
      - [Theming](#theming)
      - [Social media previews](#social-media-previews)
      - [Atom (RSS-like) Feed](#atom-rss-like-feed)
      - [Related posts](#related-posts)
      - [Code quality checks](#code-quality-checks-1)
      - [GDPR Cookie Consent Dialog](#gdpr-cookie-consent-dialog)
  - [FAQ](#faq-1)
  - [Contributing](#contributing-1)
    - [Maintainers](#maintainers-1)
    - [All Contributors](#all-contributors-1)
  - [Star History](#star-history-1)
  - [License](#license-1)

<!--te-->

## Installing and Deploying

For installation and deployment details please refer to [docs/INSTALL.md](docs/INSTALL.md).

## Customizing

For customization details please refer to [docs/CUSTOMIZE.md](docs/CUSTOMIZE.md).

## Plugin Ecosystem

`al-folio` is a thin starter in `v1.x`. Runtime features are plugin-owned and published as Ruby gems.

- Ownership boundaries: [docs/BOUNDARIES.md](docs/BOUNDARIES.md)
- Plugin catalog metadata: [`_data/featured_plugins.yml`](_data/featured_plugins.yml)
- Rendered plugin catalog: [alshedivat.github.io/al-folio/plugins/](https://alshedivat.github.io/al-folio/plugins/)
- Plugin catalog page source: [`_pages/plugins.md`](_pages/plugins.md)

The catalog page is deliberately kept out of the navbar (`nav: false`) so the demo site's chrome stays unchanged; reach it through the links above.

Naming convention:

- Theme-coupled plugins use `al-folio-<feature>` repos and `al_folio_<feature>` gem/plugin ids.
- Reusable plugins can use `al-<feature>` or neutral naming.

Featured plugins and bundled starter plugins are different tracks. Bundling requires explicit updates to [Gemfile](Gemfile) and [\_config.yml](_config.yml).
Plugin-owned changes should be made in the owning `al-org-dev` plugin repository, not by copying runtime assets into this starter.
The bundled v1 plugin repos are:

- [`al-folio-core`](https://github.com/al-org-dev/al-folio-core): shared layouts, includes, style/runtime primitives, and upgrade contracts
- [`al-folio-cv`](https://github.com/al-org-dev/al-folio-cv): CV rendering
- [`al-folio-distill`](https://github.com/al-org-dev/al-folio-distill): Distill layouts and runtime assets
- [`al-folio-bootstrap-compat`](https://github.com/al-org-dev/al-folio-bootstrap-compat): temporary Bootstrap compatibility runtime
- [`al-folio-upgrade`](https://github.com/al-org-dev/al-folio-upgrade): v1 upgrade audit/report/codemods
- [`al-icons`](https://github.com/al-org-dev/al-icons): icon loading
- [`al-search`](https://github.com/al-org-dev/al-search): search runtime
- [`al-citations`](https://github.com/al-org-dev/al-citations): publication/citation helpers
- [`al-ext-posts`](https://github.com/al-org-dev/al-ext-posts): external post ingestion
- [`al-analytics`](https://github.com/al-org-dev/al-analytics), [`al-comments`](https://github.com/al-org-dev/al-comments), [`al-cookie`](https://github.com/al-org-dev/al-cookie), [`al-img-tools`](https://github.com/al-org-dev/al-img-tools), [`al-math`](https://github.com/al-org-dev/al-math), [`al-charts`](https://github.com/al-org-dev/al-charts), and [`al-newsletter`](https://github.com/al-org-dev/al-newsletter): feature-specific runtime and integration behavior

## Using AI Agents

`al-folio` v1.x is designed for agent-assisted setup and migration. Agents should read [AGENTS.md](AGENTS.md) first, then use [docs/BOUNDARIES.md](docs/BOUNDARIES.md) to route changes to the starter or the owning plugin repo.

For existing customized forks, the recommended migration path is to ask an agent to use the [al-folio v1 migration skill](.agents/skills/al-folio-v1-migration/SKILL.md). The skill walks through creating a disposable migration branch, bringing site-owned content/config/data onto the v1 starter contract, running `al_folio_upgrade`, auditing local overrides, and validating the build. This is preferred over a manual file-by-file upgrade because v1 runtime ownership moved into plugins and local overrides need explicit drift tracking.

The canonical skills live in [.agents/skills/](.agents/skills/). They are also exposed through `.codex/skills/` and `.claude/skills/` symlinks for agents that discover skills from tool-specific directories.

### Codex

Codex can use the repo-local skills:

- [al-folio bootstrap](.agents/skills/al-folio-bootstrap/SKILL.md): create and configure a new v1 site.
- [al-folio v1 migration](.agents/skills/al-folio-v1-migration/SKILL.md): migrate customized forks and audit local overrides.

Useful first prompts:

- "Use the al-folio bootstrap skill to configure my new site."
- "Use the al-folio v1 migration skill to migrate this customized fork and run the override audit."

### Claude

Claude should start from [CLAUDE.md](CLAUDE.md), which imports [AGENTS.md](AGENTS.md). For setup or migration tasks, use the matching skill from `.claude/skills/`, which points to the canonical `.agents/skills/` directory.

### Copilot And Other Agents

Copilot should follow [.github/copilot-instructions.md](.github/copilot-instructions.md) and the specialized agents in [.github/agents/](.github/agents/). Other agents should follow the same rule: keep starter work in this repo, route runtime behavior to the owning `al-org-dev` plugin, and run `bundle exec al-folio upgrade overrides audit` whenever local overrides are added or retained.

## Documentation

Comprehensive guides for all aspects of your al-folio website:

- **[Documentation index](docs/README.md)** – All user, maintainer, and migration guides
- **[Quick Start](docs/QUICKSTART.md)** – Get running in 5 minutes
- **[Installation & Deployment](docs/INSTALL.md)** – Set up your site on GitHub Pages or other platforms
- **[Customization Guide](docs/CUSTOMIZE.md)** – Personalize your website (CVs, publications, themes, etc.)
- **[Troubleshooting](docs/TROUBLESHOOTING.md)** – Fix common issues (deployment, build, styling, content)
- **[FAQ](docs/FAQ.md)** – Frequently asked questions and solutions
- **[Analytics](docs/ANALYTICS.md)** – Add website analytics and visitor tracking
- **[SEO Guide](docs/SEO.md)** – Optimize for search engines and improve discoverability
- **[Plugin Catalog](https://alshedivat.github.io/al-folio/plugins/)** – Featured and bundled plugin metadata ([page source](_pages/plugins.md))

## Features

Everything below ships with the starter. Rows marked **setup** render nothing until you supply a key, ID or credential — bundling a plugin is not the same as switching the feature on. Each feature is owned by a versioned plugin — see [`docs/BOUNDARIES.md`](docs/BOUNDARIES.md) for the full ownership table, and [Plugin Ecosystem](#plugin-ecosystem) for how to add or remove one.

| Feature                                                                         | Plugin                           | Configure                                                                           |
| ------------------------------------------------------------------------------- | -------------------------------- | ----------------------------------------------------------------------------------- |
| Pages, layouts, navigation, light/dark mode, theming                            | `al_folio_core`                  | [Changing theme color](docs/CUSTOMIZE.md#changing-theme-color)                      |
| Publications from BibTeX                                                        | `al_folio_core` + jekyll-scholar | [Adding a new publication](docs/CUSTOMIZE.md#adding-a-new-publication)              |
| CV from RenderCV or JSONResume                                                  | `al_folio_cv`                    | [Modifying the CV information](docs/CUSTOMIZE.md#modifying-the-cv-information)      |
| Distill-style posts                                                             | `al_folio_distill`               | [the example post](https://alshedivat.github.io/al-folio/blog/2021/distill/)        |
| Math, TikZ diagrams                                                             | `al_math`                        | [the math post](https://alshedivat.github.io/al-folio/blog/2015/math/)              |
| Charts, mermaid, plotly                                                         | `al_charts`                      | [the charts post](https://alshedivat.github.io/al-folio/blog/2025/plotly/)          |
| Image zoom, galleries, sliders, lightbox                                        | `al_img_tools`                   | [the images post](https://alshedivat.github.io/al-folio/blog/2024/advanced-images/) |
| Full-text search (<kbd>ctrl</kbd> <kbd>k</kbd>)                                 | `al_search`                      | `search_enabled` in [\_config.yml](_config.yml)                                     |
| Comments (Giscus or Disqus) — **setup**                                         | `al_comments`                    | `giscus:` in [\_config.yml](_config.yml)                                            |
| Analytics — Google, Cronitor, Pirsch, Openpanel, Cloudflare, Simple — **setup** | `al_analytics`                   | [docs/ANALYTICS.md](docs/ANALYTICS.md)                                              |
| GDPR cookie consent, gating analytics until opt-in — **setup**                  | `al_cookie`                      | [GDPR Cookie Consent Dialog](docs/CUSTOMIZE.md#gdpr-cookie-consent-dialog)          |
| Newsletter signup — **setup**                                                   | `al_newsletter`                  | `newsletter:` in [\_config.yml](_config.yml)                                        |
| Citation counts, altmetric/dimensions badges                                    | `al_citations`                   | [Adding a new publication](docs/CUSTOMIZE.md#adding-a-new-publication)              |
| FontAwesome, Academicons, scholar icons                                         | `al_icons`                       | `third_party_libraries` in [\_config.yml](_config.yml)                              |
| Posts syndicated from Medium and other feeds                                    | `al_ext_posts`                   | `external_sources:` in [\_config.yml](_config.yml)                                  |
| Legacy Bootstrap markup (opt-in, removed in v2.0)                               | `al_folio_bootstrap_compat`      | `al_folio.compat.bootstrap` in [\_config.yml](_config.yml)                          |
| Upgrade audits and codemods                                                     | `al_folio_upgrade`               | `bundle exec al-folio upgrade audit`                                                |

Also included: Open Graph and schema.org previews, an Atom feed at `/feed.xml`, related posts, tabbed content, typograms, responsive image generation, and a Google Scholar citation-refresh workflow.

### Light and dark mode

The theme follows the visitor's system preference and can be toggled with the sun/moon control in the navbar. The choice persists across visits.

<p align="center">
<img src="readme_preview/light.png" width=400>
<img src="readme_preview/dark.png" width=400>
</p>

---

### The pages you get out of the box

Publications are generated from your BibTeX bibliography, the CV from a single `cv.yml` or `resume.json`, and the people page from `_data`. Everything is content-driven — you edit data files, not templates.

<p align="center">
  <a href="https://alshedivat.github.io/al-folio/publications/"><img src="readme_preview/publications.png" width=400></a>
  <a href="https://alshedivat.github.io/al-folio/cv/"><img src="readme_preview/cv.png" width=400></a>
</p>
<p align="center">
  <a href="https://alshedivat.github.io/al-folio/projects/"><img src="readme_preview/projects.png" width=400></a>
  <a href="https://alshedivat.github.io/al-folio/people/"><img src="readme_preview/people.png" width=400></a>
</p>

Projects are one of four Jekyll `collections` the starter ships (`news`, `projects`, `books`, `teachings`). You can add your own for courses, talks, or anything else — see [Adding Collections](docs/CUSTOMIZE.md#adding-collections).

---

### Writing

Posts support the [distill.pub](https://distill.pub/) layout, MathJax and TikZ, syntax-highlighted code, Jupyter notebooks, charts, image galleries, video and audio embeds.

<p align="center">
  <a href="https://alshedivat.github.io/al-folio/blog/2021/distill/"><img src="readme_preview/distill.png" width=400></a>
  <a href="https://alshedivat.github.io/al-folio/blog/2015/math/"><img src="readme_preview/math.png" width=400></a>
</p>
<p align="center">
  <a href="https://alshedivat.github.io/al-folio/blog/2015/code/"><img src="readme_preview/code.png" width=400></a>
  <a href="https://alshedivat.github.io/al-folio/projects/1_project/"><img src="readme_preview/photos-screenshot.png" width=400></a>
</p>

---

### GitHub repositories and stats

The `/repositories/` page renders repository and profile cards via [github-stats-extended](https://github.com/stats-organization/github-stats-extended). Profile trophies via [github-profile-trophy](https://github.com/ryo-ma/github-profile-trophy) are supported but **off by default**, because that project's free public instance is currently disabled — see [docs/CUSTOMIZE.md](docs/CUSTOMIZE.md#why-trophies-are-off-by-default) to self-host and re-enable.

<p align="center">
  <a href="https://alshedivat.github.io/al-folio/repositories/"><img src="readme_preview/repositories.png" width="75%"></a>
</p>

Configure which repositories and profiles appear under [Modifying the user and repository information](docs/CUSTOMIZE.md#modifying-the-user-and-repository-information).

## User community

Academics around the world use **al-folio** for their homepages, blogs, and lab pages, as well as webpages for courses, workshops, conferences, meetups, and more.

**[Browse the showcase &rarr;](docs/SHOWCASE.md)**

Want your site listed? Post a request in the _Showcase_ category of [GitHub Discussions](https://github.com/alshedivat/al-folio/discussions) — we review and add entries periodically. Please do not open a pull request for this.

## Lighthouse PageSpeed Insights

### Desktop

[![Google Lighthouse PageSpeed Insights](lighthouse_results/desktop/pagespeed.svg)](https://htmlpreview.github.io/?https://github.com/alshedivat/al-folio/blob/main/lighthouse_results/desktop/alshedivat_github_io_al_folio_.html)

Run the test yourself: [Google Lighthouse PageSpeed Insights](https://pagespeed.web.dev/report?url=https%3A%2F%2Falshedivat.github.io%2Fal-folio%2F&form_factor=desktop)

### Mobile

[![Google Lighthouse PageSpeed Insights](lighthouse_results/mobile/pagespeed.svg)](https://htmlpreview.github.io/?https://github.com/alshedivat/al-folio/blob/main/lighthouse_results/mobile/alshedivat_github_io_al_folio_.html)

Run the test yourself: [Google Lighthouse PageSpeed Insights](https://pagespeed.web.dev/report?url=https%3A%2F%2Falshedivat.github.io%2Fal-folio%2F&form_factor=mobile)

## FAQ

For frequently asked questions, please refer to [docs/FAQ.md](docs/FAQ.md).

## Contributing

Contributions to al-folio are very welcome! Before you get started, please take a look at [the guidelines](docs/CONTRIBUTING.md).

If you would like to improve documentation or fix a minor inconsistency or bug, please feel free to send a PR directly to `main`. For more complex issues/bugs or feature requests, please open an issue using the appropriate template.

### Code quality checks

CI runs the following on every pull request:

- [Prettier](https://prettier.io/) — formatting, including Liquid templates
- [lychee](https://lychee.cli.rs/) — broken links
- `npm run lint:style-contract` — enforces the thin-starter boundary described in [AGENTS.md](AGENTS.md)
- the six `test/integration_*.sh` scripts, and Playwright visual-regression checks

[Axe](https://github.com/dequelabs/axe-core) accessibility checks are run manually, because the fixes are not always straightforward for contributors without web development experience.

### Maintainers

Our most active contributors are welcome to join the maintainers team. If you are interested, please reach out!

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tbody>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="https://maruan.alshedivat.com"><img src="https://avatars.githubusercontent.com/u/2126561?v=4" width="100px;" alt=""/><br /><sub><b>Maruan</b></sub></a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://rohandebsarkar.github.io"><img src="https://avatars.githubusercontent.com/u/50144004?v=4" width="100px;" alt=""/><br /><sub><b>Rohan Deb Sarkar</b></sub></a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://amirpourmand.ir"><img src="https://avatars.githubusercontent.com/u/32064808?v=4" width="100px;" alt=""/><br /><sub><b>Amir Pourmand</b></sub></a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://george-gca.github.io/"><img src="https://avatars.githubusercontent.com/u/31376482?v=4" width="100px;" alt=""/><br /><sub><b>George</b></sub></a></td>
    </tr>
  </tbody>
</table>

<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->

### All Contributors

<a href="https://contrib.rocks">
  <img src="https://contrib.rocks/image?repo=alshedivat/al-folio&max=500&columns=24" />
</a>

## Star History

<a href="https://github.com/alshedivat/al-folio/stargazers">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/img/star-history-dark.svg" />
    <source media="(prefers-color-scheme: light)" srcset="assets/img/star-history-light.svg" />
    <img alt="Star history chart for alshedivat/al-folio" src="assets/img/star-history-light.svg" width="820" />
  </picture>
</a>

<sub>Generated by [`bin/generate_star_history.py`](bin/generate_star_history.py) and refreshed automatically by [`star-history.yml`](.github/workflows/star-history.yml).</sub>

## License

al-folio is available as open source under the terms of the [MIT License](https://github.com/alshedivat/al-folio/blob/main/LICENSE).

Originally, **al-folio** was based on the [\*folio theme](https://github.com/bogoli/-folio) (published by [Lia Bogoev](https://liabogoev.com) and under the MIT license). Since then, it got a full re-write of the styles and many additional cool features.

# al-folio

<div align="center">

[![Preview](readme_preview/al-folio-preview.png)](https://alshedivat.github.io/al-folio/)

**A simple, clean, and responsive [Jekyll](https://jekyllrb.com/) theme for academics.**

---

[![deploy](https://github.com/alshedivat/al-folio/actions/workflows/deploy.yml/badge.svg)](https://github.com/alshedivat/al-folio/actions/workflows/deploy.yml)
[![Maintainers](https://img.shields.io/badge/maintainers-4-success.svg)](#maintainers)
[![GitHub contributors](https://img.shields.io/github/contributors/alshedivat/al-folio.svg)](https://github.com/alshedivat/al-folio/graphs/contributors/)

[![Docker Image Version](https://img.shields.io/docker/v/amirpourmand/al-folio?sort=semver&label=docker%20image&color=blueviolet)](https://hub.docker.com/r/amirpourmand/al-folio)
[![Docker Image Size](https://img.shields.io/docker/image-size/amirpourmand/al-folio?sort=date&label=docker%20image%20size&color=blueviolet)](https://hub.docker.com/r/amirpourmand/al-folio)
[![Docker Pulls](https://img.shields.io/docker/pulls/amirpourmand/al-folio?color=blueviolet)](https://hub.docker.com/r/amirpourmand/al-folio)

[![GitHub release](https://img.shields.io/github/v/release/alshedivat/al-folio)](https://github.com/alshedivat/al-folio/releases/latest)
[![GitHub license](https://img.shields.io/github/license/alshedivat/al-folio?color=blue)](https://github.com/alshedivat/al-folio/blob/main/LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/alshedivat/al-folio)](https://github.com/alshedivat/al-folio/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/alshedivat/al-folio)](https://github.com/alshedivat/al-folio/fork)

[![Code Wiki](https://img.shields.io/badge/Code_Wiki-ask_about_repo-blue?logo=googlegemini)](https://codewiki.google/github.com/alshedivat/al-folio)
[![DeepWiki](https://img.shields.io/badge/DeepWiki-ask_about_repo-lightcyan)](https://deepwiki.com/alshedivat/al-folio)

</div>

## User community

The vibrant community of **al-folio** users is growing!
Academics around the world use this theme for their homepages, blogs, lab pages, as well as webpages for courses, workshops, conferences, meetups, and more.
Check out the community webpages below.
Feel free to add your own page(s) by sending a PR.

<table>
<tr>
<td>Academics</td>
<td>
<a href="https://martinbulla.github.io" target="_blank">★</a>
<a href="https://maruan.alshedivat.com" target="_blank">★</a>
<a href="https://www.cs.columbia.edu/~chen1ru/" target="_blank">★</a>
<a href="https://maithraraghu.com" target="_blank">★</a>
<a href="https://platanios.org" target="_blank">★</a>
<a href="https://otiliastr.github.io" target="_blank">★</a>
<a href="https://www.maths.dur.ac.uk/~sxwc62/" target="_blank">★</a>
<a href="https://jessachandler.com/" target="_blank">★</a>
<a href="https://mayankm96.github.io/" target="_blank">★</a>
<a href="https://markdean.info/" target="_blank">★</a>
<a href="https://kakodkar.github.io/" target="_blank">★</a>
<a href="https://sahirbhatnagar.com/" target="_blank">★</a>
<a href="https://spd.gr/" target="_blank">★</a>
<a href="https://jay-sarkar.github.io/" target="_blank">★</a>
<a href="https://aborowska.github.io/" target="_blank">★</a>
<a href="https://aditisgh.github.io/" target="_blank">★</a>
<a href="https://alexhaydock.co.uk/" target="_blank">★</a>
<a href="https://alixkeener.net/" target="_blank">★</a>
<a href="https://andreea7b.github.io/" target="_blank">★</a>
<a href="https://rishabhjoshi.github.io/" target="_blank">★</a>
<a href="https://sheelabhadra.github.io/" target="_blank">★</a>
<a href="https://giograno.me/" target="_blank">★</a>
<a href="https://immsrini.github.io/" target="_blank">★</a>
<a href="https://apooladian.github.io/" target="_blank">★</a>
<a href="https://chinmoy-dutta.github.io/" target="_blank">★</a>
<a href="https://liamcli.com/" target="_blank">★</a>
<a href="https://yoonholee.com/" target="_blank">★</a>
<a href="https://zrqiao.github.io/" target="_blank">★</a>
<a href="https://abstractgeek.github.io/" target="_blank">★</a>
<a href="https://www.compphys.de/" target="_blank">★</a>
<a href="https://julianstreyczek.github.io" target="_blank">★</a>
<a href="https://sdaza.com" target="_blank">★</a>
<a href="https://niweera.gq" target="_blank">★</a>
<a href="https://www.alihkw.com" target="_blank">★</a>
<a href="https://amirpourmand.ir" target="_blank">★</a>
<a href="https://scottleechua.github.io" target="_blank">★</a>
<a href="https://sk1y101.github.io" target="_blank">★</a>
<a href="https://yyang768osu.github.io" target="_blank">★</a>
<a href="https://veedata.github.io" target="_blank">★</a>
<a href="https://K-Wu.github.io" target="_blank">★</a>
<a href="https://amalawilson.com" target="_blank">★</a>
<a href="https://tirtharajdash.github.io" target="_blank">★</a>
<a href="https://carolinacarreira.github.io" target="_blank">★</a>
<a href="https://manandey.github.io" target="_blank">★</a>
<a href="https://johanneshoerner.github.io" target="_blank">★</a>
<a href="https://ioannismavromatis.com" target="_blank">★</a>
<a href="https://taidnguyen.github.io" target="_blank">★</a>
<a href="https://lbugnon.github.io" target="_blank">★</a>
<a href="https://joahannes.github.io" target="_blank">★</a>
<a href="https://dominikstrb.github.io" target="_blank">★</a>
<a href="https://tylerbarna.com" target="_blank">★</a>
<a href="https://daviddmc.github.io/" target="_blank">★</a>
<a href="https://andreaskuster.ch/" target="_blank">★</a>
<a href="https://ellisbrown.github.io/" target="_blank">★</a>
<a href="https://djherron.github.io/" target="_blank">★</a>
<a href="https://rodosingh.github.io/" target="_blank">★</a>
<a href="https://vdivakar.github.io/" target="_blank">★</a>
<a href="https://george-gca.github.io/" target="_blank">★</a>
<a href="https://bashirkazimi.github.io/" target="_blank">★</a>
<a href="https://dohaison.github.io/" target="_blank">★</a>
<a href="https://raphaaal.github.io/" target="_blank">★</a>
<a href="https://varuniyer.info/" target="_blank">★</a>
<a href="https://yukimasano.github.io/" target="_blank">★</a>
<a href="https://hashe037.github.io/" target="_blank">★</a>
<a href="https://wang-boyu.github.io/" target="_blank">★</a>
<a href="https://qingqingchen.info" target="_blank">★</a>
<a href="https://bajinsheng.github.io/" target="_blank">★</a>
<a href="https://www.silviofanzon.com/" target="_blank">★</a>
<a href="https://kaikaiyao.github.io/" target="_blank">★</a>
<a href="https://alchemz.github.io/" target="_blank">★</a>
<a href="https://samadamday.com/" target="_blank">★</a>
<a href="https://fanpu.io/" target="_blank">★</a>
<a href="https://abigalekim.github.io/" target="_blank">★</a>
<a href="https://lucasresck.github.io/" target="_blank">★</a>
<a href="https://users.wpi.edu/~lfichera/" target="_blank">★</a>
<a href="https://anmspro.github.io/" target="_blank">★</a>
<a href="https://berlyne.net/" target="_blank">★</a>
<a href="https://filippomazzoli.github.io/" target="_blank">★</a>
<a href="https://www.escontrela.me/" target="_blank">★</a>
<a href="https://raffaem.github.io/" target="_blank">★</a>
<a href="https://cbueth.de/" target="_blank">★</a>
<a href="https://kyleaoman.github.io/" target="_blank">★</a>
<a href="https://decwest.github.io/" target="_blank">★</a>
<a href="https://www.jedburkat.com" target="_blank">★</a>
<a href="https://hrzhang.me" target="_blank">★</a>
<a href="https://kudhru.github.io/" target="_blank">★</a>
<a href="https://mbarbetti.github.io/" target="_blank">★</a>
<a href="https://www.zhivotenko.com/" target="_blank">★</a>
<a href="https://giordanodaloisio.github.io/" target="_blank">★</a>
<a href="https://aadityaura.github.io/" target="_blank">★</a>
<a href="https://abhinav-mehta.github.io/" target="_blank">★</a>
<a href="https://shubhashisroydipta.com/" target="_blank">★</a>
<a href="https://astanziola.github.io" target="_blank">★</a>
<a href="https://tinkerer.in" target="_blank">★</a>
<a href="https://afraniomelo.github.io/en/" target="_blank">★</a>
<a href="https://jonaruthardt.github.io" target="_blank">★</a>
<a href="https://www.zla.app/" target="_blank">★</a>
<a href="https://stavros.github.io" target="_blank">★</a>
<a href="https://ericslyman.com" target="_blank">★</a>
<a href="https://ztjona.github.io/" target="_blank">★</a>
<a href="https://chrischoi314.github.io" target="_blank">★</a>
<a href="https://riccobelli.faculty.polimi.it" target="_blank">★</a>
<a href="https://kishanved.tech/" target="_blank">★</a>
<a href="https://abhilesh.github.io/" target="_blank">★</a>
<a href="https://jackjburnett.github.io/" target="_blank">★</a>
<a href="https://physics-morris.github.io/" target="_blank">★</a>
<a href="https://sraf.ir" target="_blank">★</a>
<a href="https://acad.garywei.dev/" target="_blank">★</a>
<a href="https://tonideleo.github.io/" target="_blank">★</a>
<a href="https://alonkellner.com/" target="_blank">★</a>
<a href="https://berylbir.github.io/" target="_blank">★</a>
<a href="https://global-anomaly.github.io/" target="_blank">★</a>
<a href="https://mingsun-kaust.github.io/" target="_blank">★</a>
<a href="https://hdocmsu.github.io/" target="_blank">★</a>
<a href="https://trandangtrungduc.github.io/" target="_blank">★</a>
<a href="https://kinghowler.github.io/" target="_blank">★</a>
<a href="https://anurye.github.io/" target="_blank">★</a>
<a href="https://charlie-xiao.github.io/" target="_blank">★</a>
<a href="https://giuseppeperelli.github.io/" target="_blank">★</a>
<a href="https://shlee-lab.github.io/" target="_blank">★</a>
<a href="https://devos50.github.io/" target="_blank">★</a>
<a href="https://vmooers.github.io/" target="_blank">★</a>
<a href="https://jpfonseca.github.io/" target="_blank">★</a>
<a href="https://dmitryryumin.github.io/" target="_blank">★</a>
<a href="https://alexiglad.github.io/" target="_blank">★</a>
<a href="https://nishanthjkumar.com/" target="_blank">★</a>
<a href="https://joszuijderwijk.nl/" target="_blank">★</a>
<a href="https://d-jiao.github.io/" target="_blank">★</a>
<a href="https://cbuelt.github.io/" target="_blank">★</a>
<a href="https://mehrdad-noori.github.io/" target="_blank">★</a>
<a href="https://arthurclerjon.github.io/" target="_blank">★</a>
<a href="https://eilamshapira.com/" target="_blank">★</a>
<a href="https://freifrauvonbleifrei.github.io/" target="_blank">★</a>
<a href="https://thomasbourke1.github.io/" target="_blank">★</a>
<a href="https://siddharthsule.com/" target="_blank">★</a>
<a href="https://waynexucn.github.io/" target="_blank">★</a>
<a href="https://zlatanajanovic.com/" target="_blank">★</a>
<a href="https://mchadolias.github.io/" target="_blank">★</a>
<a href="https://syanyong.github.io/" target="_blank">★</a>
<a href="https://jucheval.github.io/" target="_blank">★</a>
<a href="https://j1yoo.github.io/" target="_blank">★</a>
<a href="https://zhoji.github.io/" target="_blank">★</a>
<a href="https://smsnobin77.github.io/" target="_blank">★</a>
<a href="https://dongkyu-lee.info/" target="_blank">★</a>
</td>
</tr>
<tr>
<td>Labs</td>
<td>
<a href="https://www.haylab.caltech.edu/" target="_blank">★</a>
<a href="https://sjkimlab.github.io/" target="_blank">★</a>
<a href="https://systemconsultantgroup.github.io/scg-folio/" target="_blank">★</a>
<a href="https://decisionlab.ucsf.edu/" target="_blank">★</a>
<a href="https://programming-group.com/" target="_blank">★</a>
<a href="https://sailing-lab.github.io/" target="_blank">★</a>
<a href="https://inbt.jhu.edu/epidiagnostics/" target="_blank">★</a>
<a href="https://www.nuesl.org/" target="_blank">★</a>
<a href="https://big-culture.github.io/" target="_blank">★</a>
<a href="https://martinbulla.github.io/bullab/" target="_blank">★</a>
<a href="https://gpforesteyes.github.io/" target="_blank">★</a>
</td>
</tr>
<tr>
<td>Courses</td>
<td>
CMU PGM (<a href="https://sailinglab.github.io/pgm-spring-2019/" target="_blank">S-19</a>) <br>
CMU DeepRL (<a href="https://cmudeeprl.github.io/403_website/" target="_blank">S-21</a>, <a href="https://cmudeeprl.github.io/703website_f21/" target="_blank">F-21</a>, <a href="https://cmudeeprl.github.io/403website_s22/" target="_blank">S-22</a>, <a href="https://cmudeeprl.github.io/703website_f22/" target="_blank">F-22</a>, <a href="https://cmudeeprl.github.io/403website_s23/" target="_blank">S-23</a>, <a href="https://cmudeeprl.github.io/703website_f23/" target="_blank">F-23</a>) <br>
CMU MMML (<a href="https://cmu-multicomp-lab.github.io/mmml-course/fall2020/" target="_blank">F-20</a>, <a href="https://cmu-multicomp-lab.github.io/mmml-course/fall2022/" target="_blank">F-22</a>) <br>
CMU AMMML (<a href="https://cmu-multicomp-lab.github.io/adv-mmml-course/spring2022/" target="_blank">S-22</a>, <a href="https://cmu-multicomp-lab.github.io/adv-mmml-course/spring2023/" target="_blank">S-23</a>) <br>
CMU ASI (<a href="https://cmu-multicomp-lab.github.io/asi-course/spring2023/" target="_blank">S-23</a>) <br>
CMU Distributed Systems (<a href="https://andrew.cmu.edu/course/15-440/" target="_blank">S-24</a>)
</td>
</tr>
<tr>
<td>Conferences & workshops</td>
<td>
ICLR Blog Post Track (<a href="https://iclr-blogposts.github.io/2023/" target="_blank">2023</a>, <a href="https://iclr-blogposts.github.io/2024/about" target="_blank">2024</a>) <br>
ML Retrospectives (NeurIPS: <a href="https://ml-retrospectives.github.io/neurips2019/" target="_blank">2019</a>, <a href="https://ml-retrospectives.github.io/neurips2020/" target="_blank">2020</a>; ICML: <a href="https://ml-retrospectives.github.io/icml2020/" target="_blank">2020</a>) <br>
HAMLETS (NeurIPS: <a href="https://hamlets-workshop.github.io/" target="_blank">2020</a>) <br>
ICBINB (NeurIPS: <a href="https://i-cant-believe-its-not-better.github.io/" target="_blank">2020</a>, <a href="https://i-cant-believe-its-not-better.github.io/neurips2021/" target="_blank">2021</a>) <br>
Neural Compression (ICLR: <a href="https://neuralcompression.github.io/" target="_blank">2021</a>) <br>
Score Based Methods (NeurIPS: <a href="https://score-based-methods-workshop.github.io/" target="_blank">2022</a>)<br>
Images2Symbols (CogSci: <a href="https://images2symbols.github.io/" target="_blank"> 2022</a>) <br>
Medical Robotics Junior Faculty Forum (ISMR: <a href="https://junior-forum-ismr.github.io/" target="_blank"> 2023</a>)<br>
Beyond Vision: Physics meets AI (ICIAP: <a href="https://physicsmeetsai.github.io/beyond-vision/" target="_blank">2023</a>) <br>
Workshop on Diffusion Models (NeurIPS: <a href="https://diffusionworkshop.github.io/" target="_blank">2023</a>) <br>
Workshop on Structured Probabilistic Inference & Generative Modeling (ICML: <a href="https://spigmworkshop.github.io/" target="_blank">2023</a>, <a href="https://spigmworkshop2024.github.io/" target="_blank">2024</a>)
</td>
</tr>
</table>

## Lighthouse PageSpeed Insights

### Desktop

[![Google Lighthouse PageSpeed Insights](lighthouse_results/desktop/pagespeed.svg)](https://htmlpreview.github.io/?https://github.com/alshedivat/al-folio/blob/main/lighthouse_results/desktop/alshedivat_github_io_al_folio_.html)

Run the test yourself: [Google Lighthouse PageSpeed Insights](https://pagespeed.web.dev/report?url=https%3A%2F%2Falshedivat.github.io%2Fal-folio%2F&form_factor=desktop)

### Mobile

[![Google Lighthouse PageSpeed Insights](lighthouse_results/mobile/pagespeed.svg)](https://htmlpreview.github.io/?https://github.com/alshedivat/al-folio/blob/main/lighthouse_results/mobile/alshedivat_github_io_al_folio_.html)

Run the test yourself: [Google Lighthouse PageSpeed Insights](https://pagespeed.web.dev/report?url=https%3A%2F%2Falshedivat.github.io%2Fal-folio%2F&form_factor=mobile)

## Table Of Contents

<!--ts-->

- [al-folio](#al-folio)
  - [Getting started](#getting-started)
  - [Table Of Contents](#table-of-contents)
  - [Installing and Deploying](#installing-and-deploying)
  - [Customizing](#customizing)
  - [Plugin Ecosystem](#plugin-ecosystem)
  - [Using AI Agents](#using-ai-agents)
    - [Codex](#codex)
    - [Claude](#claude)
    - [Copilot And Other Agents](#copilot-and-other-agents)
  - [Documentation](#documentation)
  - [Features](#features)
    - [Light and dark mode](#light-and-dark-mode)
    - [The pages you get out of the box](#the-pages-you-get-out-of-the-box)
    - [Writing](#writing)
    - [GitHub repositories and stats](#github-repositories-and-stats)
  - [User community](#user-community)
  - [Lighthouse PageSpeed Insights](#lighthouse-pagespeed-insights)
    - [Desktop](#desktop)
    - [Mobile](#mobile)
  - [FAQ](#faq)
  - [Contributing](#contributing)
    - [Code quality checks](#code-quality-checks)
    - [Maintainers](#maintainers)
    - [All Contributors](#all-contributors)
  - [Star History](#star-history)
  - [License](#license)
- [al-folio](#al-folio-1)
  - [User community](#user-community-1)
  - [Lighthouse PageSpeed Insights](#lighthouse-pagespeed-insights-1)
    - [Desktop](#desktop-1)
    - [Mobile](#mobile-1)
  - [Table Of Contents](#table-of-contents-1)
  - [Getting started](#getting-started-1)
  - [Installing and Deploying](#installing-and-deploying-1)
  - [Customizing](#customizing-1)
  - [GitHub Copilot Agents](#github-copilot-agents)
    - [Customization Agent](#customization-agent)
    - [Documentation Agent](#documentation-agent)
  - [Documentation](#documentation-1)
  - [Features](#features-1)
    - [Light/Dark Mode](#lightdark-mode)
    - [CV](#cv)
    - [People](#people)
    - [Publications](#publications)
    - [Collections](#collections)
    - [Layouts](#layouts)
      - [The iconic style of Distill](#the-iconic-style-of-distill)
      - [Full support for math &amp; code](#full-support-for-math--code)
      - [Photos, Audio, Video and more](#photos-audio-video-and-more)
    - [Other features](#other-features)
      - [GitHub's repositories and user stats](#githubs-repositories-and-user-stats)
      - [Theming](#theming)
      - [Social media previews](#social-media-previews)
      - [Atom (RSS-like) Feed](#atom-rss-like-feed)
      - [Related posts](#related-posts)
      - [Code quality checks](#code-quality-checks-1)
      - [GDPR Cookie Consent Dialog](#gdpr-cookie-consent-dialog)
  - [FAQ](#faq-1)
  - [Contributing](#contributing-1)
    - [Maintainers](#maintainers-1)
    - [All Contributors](#all-contributors-1)
  - [Star History](#star-history-1)
  - [License](#license-1)

<!--te-->

## Getting started

**⚠️ Important: Use "Use this template" (not fork)**

When creating your own website with al-folio, you have two options:

- ✅ **Recommended:** Click "[Use this template](https://github.com/new?template_name=al-folio&template_owner=alshedivat)" – This creates a clean copy that is independent from the main al-folio repository. Changes you make to your site won't be accidentally submitted to al-folio as pull requests.
- ❌ **Not recommended:** Forking the repository – This keeps a link to the main al-folio repo, making it easy to accidentally submit your personal site changes as contributions to our project.

**If you already forked:** Don't worry! You can still work with your fork normally. Just make sure to:

1. Make changes on a dedicated branch (e.g., `my-site-updates`)
2. When pushing changes, always verify you're pushing to **your own repository**, not the main al-folio repository
3. Never create pull requests to `alshedivat/al-folio` unless you're intentionally contributing improvements that benefit all users

For quick setup, see [QUICKSTART.md](QUICKSTART.md).

Want to learn more about Jekyll? Check out [this tutorial](https://www.taniarascia.com/make-a-static-website-with-jekyll/). Why Jekyll? Read [Andrej Karpathy's blog post](https://karpathy.github.io/2014/07/01/switching-to-jekyll/)! Why write a blog? Read [Rachel Thomas blog post](https://medium.com/@racheltho/why-you-yes-you-should-blog-7d2544ac1045).

## Installing and Deploying

For installation and deployment details please refer to [INSTALL.md](INSTALL.md).

## Customizing

For customization details please refer to [CUSTOMIZE.md](CUSTOMIZE.md).

## GitHub Copilot Agents

This repository includes two specialized GitHub Copilot agents to enhance your development experience:

### Customization Agent

The **Customization Agent** helps you personalize your al-folio website by:

- Guiding you through configuration changes step-by-step
- Modifying files directly in your repository
- Explaining technical concepts in plain language (great for users without coding experience)
- Assisting with common tasks like updating your CV, adding publications, creating blog posts, and customizing themes

See [CUSTOMIZE.md § GitHub Copilot Customization Agent](CUSTOMIZE.md#github-copilot-customization-agent) for detailed usage instructions.

### Documentation Agent

The **Documentation Agent** maintains clear and up-to-date project documentation by:

- Updating documentation files when features change
- Writing in a style accessible to academics and researchers
- Keeping documentation synchronized with the codebase
- Following documentation best practices

See [CONTRIBUTING.md § GitHub Copilot Agents](CONTRIBUTING.md#github-copilot-agents) for more information.

> **Requirements:** Both agents require a [GitHub Copilot](https://github.com/features/copilot) subscription. For more information about GitHub Copilot and how to use agents, see the [GitHub Copilot documentation](https://docs.github.com/en/copilot).

## Documentation

Comprehensive guides for all aspects of your al-folio website:

- **[Quick Start](QUICKSTART.md)** – Get running in 5 minutes
- **[Installation & Deployment](INSTALL.md)** – Set up your site on GitHub Pages or other platforms
- **[Customization Guide](CUSTOMIZE.md)** – Personalize your website (CVs, publications, themes, etc.)
- **[Troubleshooting](TROUBLESHOOTING.md)** – Fix common issues (deployment, build, styling, content)
- **[FAQ](FAQ.md)** – Frequently asked questions and solutions
- **[Analytics](ANALYTICS.md)** – Add website analytics and visitor tracking
- **[SEO Guide](SEO.md)** – Optimize for search engines and improve discoverability

## Features

### Light/Dark Mode

This template has a built-in light/dark mode. It detects the user preferred color scheme and automatically switches to it. You can also manually switch between light and dark mode by clicking on the sun/moon icon in the top right corner of the page.

<p align="center">
<img src="readme_preview/light.png" width=400>
<img src="readme_preview/dark.png" width=400>
</p>

---

### CV

Your CV can be generated in one of two modern formats: **RenderCV** (recommended, with automatic PDF generation) or **JSONResume** (standardized JSON format). You can use both simultaneously and switch between them, or maintain just the one you prefer.

[![CV Preview](readme_preview/cv.png)](https://alshedivat.github.io/al-folio/cv/)

For setup and customization details, see [Modifying the CV information](CUSTOMIZE.md#modifying-the-cv-information) in [CUSTOMIZE.md](CUSTOMIZE.md).

---

### People

You can create a people page if you want to feature more than one person. Each person can have its own short bio, profile picture, and you can also set if every person will appear at the same or opposite sides.

[![People Preview](readme_preview/people.png)](https://alshedivat.github.io/al-folio/people/)

---

### Publications

Your publications page is generated automatically from your BibTeX bibliography. You can customize publication display, add extra information like PDFs, and control sorting behavior.

[![Publications Preview](readme_preview/publications.png)](https://alshedivat.github.io/al-folio/publications/)

For setup, BibTeX field documentation, and customization options, see [Adding a new publication](CUSTOMIZE.md#adding-a-new-publication) and [Managing publication display](CUSTOMIZE.md#managing-publication-display) in [CUSTOMIZE.md](CUSTOMIZE.md).

---

### Collections

This Jekyll theme implements `collections` to organize content into categories. The theme comes with default collections for `news`, `projects`, `books`, and `teachings`. You can easily create your own collections for apps, stories, courses, or any other creative work.

[![Projects Preview](readme_preview/projects.png)](https://alshedivat.github.io/al-folio/projects/)

For detailed instructions on creating and customizing collections, see [Adding Collections](CUSTOMIZE.md#adding-collections) in [CUSTOMIZE.md](CUSTOMIZE.md).

---

### Layouts

**al-folio** comes with stylish layouts for pages and blog posts.

#### The iconic style of Distill

The theme allows you to create blog posts in the [distill.pub](https://distill.pub/) style:

[![Distill Preview](readme_preview/distill.png)](https://alshedivat.github.io/al-folio/blog/2021/distill/)

For more details on how to create distill-styled posts using `<d-*>` tags, please refer to [the example](https://alshedivat.github.io/al-folio/blog/2021/distill/).

#### Full support for math & code

**al-folio** supports fast math typesetting through [MathJax](https://www.mathjax.org/) and code syntax highlighting using [GitHub style](https://github.com/jwarby/jekyll-pygments-themes). Also supports [chartjs charts](https://www.chartjs.org/), [mermaid diagrams](https://mermaid-js.github.io/mermaid/#/), and [TikZ figures](https://tikzjax.com/).

<p align="center">
<a href="https://alshedivat.github.io/al-folio/blog/2015/math/" target="_blank"><img src="readme_preview/math.png" width=400></a>
<a href="https://alshedivat.github.io/al-folio/blog/2015/code/" target="_blank"><img src="readme_preview/code.png" width=400></a>
</p>

#### Photos, Audio, Video and more

Photo formatting is made simple using [Bootstrap's grid system](https://getbootstrap.com/docs/4.4/layout/grid/). Easily create beautiful grids within your blog posts and project pages, also with support for [video](https://alshedivat.github.io/al-folio/blog/2023/videos/) and [audio](https://alshedivat.github.io/al-folio/blog/2023/audios/) embeds:

<p align="center">
  <a href="https://alshedivat.github.io/al-folio/projects/1_project/">
    <img src="readme_preview/photos-screenshot.png" width="75%">
  </a>
</p>

---

### Other features

#### GitHub's repositories and user stats

**al-folio** displays GitHub repositories and user stats on the `/repositories/` page using [github-readme-stats](https://github.com/anuraghazra/github-readme-stats) and [github-profile-trophy](https://github.com/ryo-ma/github-profile-trophy).

[![Repositories Preview](readme_preview/repositories.png)](https://alshedivat.github.io/al-folio/repositories/)

To configure which repositories and GitHub profiles to display, see [Modifying the user and repository information](CUSTOMIZE.md#modifying-the-user-and-repository-information) in [CUSTOMIZE.md](CUSTOMIZE.md).

---

#### Theming

**al-folio** offers a variety of beautiful theme colors to choose from. The default is purple, but you can customize colors, fonts, spacing, and more to match your style.

For detailed customization instructions, see [Changing theme color](CUSTOMIZE.md#changing-theme-color) and [Customizing fonts, spacing, and more](CUSTOMIZE.md#customizing-fonts-spacing-and-more) in [CUSTOMIZE.md](CUSTOMIZE.md).

---

#### Social media previews

**al-folio** supports Open Graph preview images on social media. When enabled, your site's pages display rich preview objects with images, titles, and descriptions when shared.

For setup and customization, see [Social media previews](CUSTOMIZE.md#social-media-previews) in [CUSTOMIZE.md](CUSTOMIZE.md).

---

#### Atom (RSS-like) Feed

It generates an Atom (RSS-like) feed of your posts, useful for Atom and RSS readers. The feed is reachable simply by typing after your homepage `/feed.xml`. E.g. assuming your website mountpoint is the main folder, you can type `yourusername.github.io/feed.xml`

---

#### Related posts

By default, blog posts display related posts at the bottom. These are selected by finding the most recent posts that share tags with the current post. You can customize this behavior on a per-post or site-wide basis.

For configuration details, see [Related posts](CUSTOMIZE.md#related-posts) in [CUSTOMIZE.md](CUSTOMIZE.md).

---

#### Code quality checks

Currently, we run some checks to ensure that the code quality and generated site are good. The checks are done using GitHub Actions and the following tools:

- [Prettier](https://prettier.io/) - check if the formatting of the code follows the style guide
- [lychee](https://lychee.cli.rs/) - check for broken links
- [Axe](https://github.com/dequelabs/axe-core) (need to run manually) - do some accessibility testing

We decided to keep `Axe` runs manual because fixing the issues are not straightforward and might be hard for people without web development knowledge.

---

#### GDPR Cookie Consent Dialog

**al-folio** includes a built-in, GDPR-compliant cookie consent dialog to ensure your website respects visitor privacy. The dialog is powered by [Vanilla Cookie Consent](https://cookieconsent.orestbida.com/) and integrates seamlessly with all supported analytics providers.

When enabled, analytics scripts are blocked until the user explicitly consents, and user preferences are saved across visits. This is essential for websites serving visitors in the European Union and other regions with strict privacy regulations.

For complete setup and customization details, see [GDPR Cookie Consent Dialog](#gdpr-cookie-consent-dialog) in [CUSTOMIZE.md](CUSTOMIZE.md).

## FAQ

For frequently asked questions, please refer to [FAQ.md](FAQ.md).

## Contributing

Contributions to al-folio are very welcome! Before you get started, please take a look at [the guidelines](CONTRIBUTING.md).

If you would like to improve documentation or fix a minor inconsistency or bug, please feel free to send a PR directly to `main`. For more complex issues/bugs or feature requests, please open an issue using the appropriate template.

### Maintainers

Our most active contributors are welcome to join the maintainers team. If you are interested, please reach out!

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tbody>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="https://maruan.alshedivat.com"><img src="https://avatars.githubusercontent.com/u/2126561?v=4" width="100px;" alt=""/><br /><sub><b>Maruan</b></sub></a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://rohandebsarkar.github.io"><img src="https://avatars.githubusercontent.com/u/50144004?v=4" width="100px;" alt=""/><br /><sub><b>Rohan Deb Sarkar</b></sub></a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://amirpourmand.ir"><img src="https://avatars.githubusercontent.com/u/32064808?v=4" width="100px;" alt=""/><br /><sub><b>Amir Pourmand</b></sub></a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://george-gca.github.io/"><img src="https://avatars.githubusercontent.com/u/31376482?v=4" width="100px;" alt=""/><br /><sub><b>George</b></sub></a></td>
    </tr>
  </tbody>
</table>

<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->

### All Contributors

<a href="https://contrib.rocks">
  <img src="https://contrib.rocks/image?repo=alshedivat/al-folio&max=500&columns=24" />
</a>

## Star History

<a href="https://star-history.com/#alshedivat/al-folio&Date">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=alshedivat/al-folio&type=Date&theme=dark" />
    <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=alshedivat/al-folio&type=Date" />
    <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=alshedivat/al-folio&type=Date" />
  </picture>
</a>

## License

The theme is available as open source under the terms of the [MIT License](https://github.com/alshedivat/al-folio/blob/main/LICENSE).

Originally, **al-folio** was based on the [\*folio theme](https://github.com/bogoli/-folio) (published by [Lia Bogoev](https://liabogoev.com) and under the MIT license). Since then, it got a full re-write of the styles and many additional cool features.
