# Hugo SEO Module

[![Used By](https://img.shields.io/badge/dynamic/json?color=success&label=used+by&query=repositories_humanize&logo=hugo&style=flat-square&url=https://api.razonyang.com/v1/github/dependents/razonyang/hugo-mod-seo)](https://github.com/razonyang/hugo-mod-seo/network/dependents)
![Hugo Requirements](https://img.shields.io/badge/dynamic/json?color=important&label=requirements&query=requirements&logo=hugo&style=flat-square&url=https://api.razonyang.com/v1/hugo/modules/github.com/razonyang/hugo-mod-seo)
[![License](https://img.shields.io/github/license/razonyang/hugo-mod-seo?style=flat-square)](https://github.com/razonyang/hugo-mod-seo/blob/main/LICENSE)
[![Version](https://img.shields.io/github/v/tag/razonyang/hugo-mod-seo?label=version&style=flat-square)](https://github.com/razonyang/hugo-mod-seo/tags)

This module ships with some templates to helps you generate SEO stuff, such as meta tags.

## Partials

| Partial | Description
|---|---
| `hugopress/modules/seo/alternatives` | Alternative pages.
| `hugopress/modules/seo/open-graph` | [Open Graph](https://ogp.me/).
| `hugopress/modules/seo/schema` | [Schema](https://schema.org/).
| `hugopress/modules/seo/translations` | Localized pages, see [Tell Google about localized versions of your page](https://developers.google.com/search/docs/specialty/international/localized-versions).
| `hugopress/modules/seo/twitter-cards` | [Twitter Card](https://developer.twitter.com/en/docs/twitter-for-websites/cards/overview/abouts-cards).

## Usage

> Skip this section if your theme supports [HugoPress](https://github.com/razonyang/hugopress), all partials will be included automatically.

Just include the partials you want.

```go
{{ partial "hugopress/modules/seo/alternatives" . }}
{{ partial "hugopress/modules/seo/translations" . }}
{{ partial "hugopress/modules/seo/schema.html" . }}
{{ partial "hugopress/modules/seo/open-graph.html" . }}
{{ partial "hugopress/modules/seo/twitter-cards.html" . }}
```
