# Hugo SEO Module

[![Used By](https://img.shields.io/badge/dynamic/json?color=success&label=used+by&query=repositories_humanize&logo=hugo&style=flat-square&url=https://api.razonyang.com/v1/github/dependents/razonyang/hugo-mod-seo)](https://github.com/razonyang/hugo-mod-seo/network/dependents)
![Hugo Requirements](https://img.shields.io/badge/dynamic/json?color=important&label=requirements&query=requirements&logo=hugo&style=flat-square&url=https://api.razonyang.com/v1/hugo/modules/github.com/razonyang/hugo-mod-seo)
[![License](https://img.shields.io/github/license/razonyang/hugo-mod-seo?style=flat-square)](https://github.com/razonyang/hugo-mod-seo/blob/main/LICENSE)
[![Version](https://img.shields.io/github/v/tag/razonyang/hugo-mod-seo?label=version&style=flat-square)](https://github.com/razonyang/hugo-mod-seo/tags)

This module ships with some modules to helps you generate SEO stuff, such as meta tags.

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

## Modules

### Base

Set the `lang` and `dir` attributes on `<html>`.

| Path                                             | Partial |
| ------------------------------------------------ | ------- |
| `github.com/razonyang/hugo-mod-seo/modules/base` | -       |

### Alternatives

Generates alternative pages meta tags.

| Path                                                     | Partial                      |
| -------------------------------------------------------- | ---------------------------- |
| `github.com/razonyang/hugo-mod-seo/modules/alternatives` | `seo/modules/favicons/index` |

### Favicons

Generates favicons in multiple sizes base on the `assets/favicon.png`.

| Path                                                 | Partial                      |
| ---------------------------------------------------- | ---------------------------- |
| `github.com/razonyang/hugo-mod-seo/modules/favicons` | `seo/modules/favicons/index` |

- The `assets/favicon.png` for generating icons in multiple sizes by default.
- The `assets/favicon.ico` or `static/favicon.ico` for classic browsers.
- The `assets/mask-icon.svg` for Safari pinned tab by default.

The following params begin with `params.seo.favicons`.

| Params            |  Type  |     Default     | Description           |
| ----------------- | :----: | :-------------: | --------------------- |
| `icon`            | String |  `favicon.png`  |
| `mask_icon`       | String | `mask-icon.svg` |
| `mask_icon_color` | String |    `#000000`    |
| `sizes`           | Array  |        -        |
| `sizes.size`      | String |        -        | For example, `32x32`. |
| `sizes.rel`       | String |     `icon`      |

```toml
[[params.seo.favicons.sizes]]
  size = '16x16'
[[params.seo.favicons.sizes]]
  size = '32x32'
[[params.seo.favicons.sizes]]
  size = '150x150'
[[params.seo.favicons.sizes]]
  rel = 'apple-touch-icon'
  size = '180x180'
[[params.seo.favicons.sizes]]
  size = '192x192'
```

### Open Graph

[Open Graph](https://ogp.me/).

| Path                                                   | Partial                        |
| ------------------------------------------------------ | ------------------------------ |
| `github.com/razonyang/hugo-mod-seo/modules/open-graph` | `seo/modules/open-graph/index` |

### Schema

[Schema](https://schema.org/).

| Path                                               | Partial                    |
| -------------------------------------------------- | -------------------------- |
| `github.com/razonyang/hugo-mod-seo/modules/schema` | `seo/modules/schema/index` |

### Translations

Localized pages, see [Tell Google about localized versions of your page](https://developers.google.com/search/docs/specialty/international/localized-versions).

| Path                                                     | Partial                          |
| -------------------------------------------------------- | -------------------------------- |
| `github.com/razonyang/hugo-mod-seo/modules/translations` | `seo/modules/translations/index` |

### Twitter Cards

[Twitter Card](https://developer.twitter.com/en/docs/twitter-for-websites/cards/overview/abouts-cards).

| Path                                                      | Partial                           |
| --------------------------------------------------------- | --------------------------------- |
| `github.com/razonyang/hugo-mod-seo/modules/twitter-cards` | `seo/modules/twitter-cards/index` |
