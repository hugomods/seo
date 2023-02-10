# Hugo SEO Module

[![Used By](https://img.shields.io/badge/dynamic/json?color=success&label=used+by&query=repositories_humanize&logo=hugo&style=flat-square&url=https://api.razonyang.com/v1/github/dependents/razonyang/hugo-mod-seo)](https://github.com/razonyang/hugo-mod-seo/network/dependents)
![Hugo Requirements](https://img.shields.io/badge/dynamic/json?color=important&label=requirements&query=requirements&logo=hugo&style=flat-square&url=https://api.razonyang.com/v1/hugo/modules/github.com/razonyang/hugo-mod-seo)
[![License](https://img.shields.io/github/license/razonyang/hugo-mod-seo?style=flat-square)](https://github.com/razonyang/hugo-mod-seo/blob/main/LICENSE)
[![Version](https://img.shields.io/github/v/tag/razonyang/hugo-mod-seo?label=version&style=flat-square)](https://github.com/razonyang/hugo-mod-seo/tags)

This module ships with some modules to helps you generate SEO stuff, such as meta tags.

## Modules

| Module                                                    |              Partial              | Description                                                                                                                                                     |
| --------------------------------------------------------- | :-------------------------------: | --------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `github.com/razonyang/hugo-mod-seo/modules/base`          |                 -                 | Set the `lang` and `dir` attributes on `<html>`.                                                                                                                |
| `github.com/razonyang/hugo-mod-seo/modules/alternatives`  | `seo/modules/alternatives/index`  | Alternative pages.                                                                                                                                              |
| `github.com/razonyang/hugo-mod-seo/modules/open-graph`    |  `seo/modules/open-graph/index`   | [Open Graph](https://ogp.me/).                                                                                                                                  |
| `github.com/razonyang/hugo-mod-seo/modules/schema`        |    `seo/modules/schema/index`     | [Schema](https://schema.org/).                                                                                                                                  |
| `github.com/razonyang/hugo-mod-seo/modules/translations`  | `seo/modules/translations/index`  | Localized pages, see [Tell Google about localized versions of your page](https://developers.google.com/search/docs/specialty/international/localized-versions). |
| `github.com/razonyang/hugo-mod-seo/modules/twitter-cards` | `seo/modules/twitter-cards/index` | [Twitter Card](https://developer.twitter.com/en/docs/twitter-for-websites/cards/overview/abouts-cards).                                                         |

## Usage

### Import the Module

```toml
[module.imports]
path = "MODULE_PATH"
```

### Include the Partial

> Skip this section if your theme supports [HugoPress](https://github.com/razonyang/hugopress), all partials will be included automatically.

```go
{{ partial "MODULE_PARTIAL" . }}
```
