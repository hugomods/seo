# Hugo SEO Module

This module ships with some templates to helps you generate SEO stuff, such as meta tags.

## Partials

| Partial | Description
|---|---
| `hugopress/modules/seo/all` | Include all of the SEO partials.
| `hugopress/modules/seo/alternatives` | Alternative pages.
| `hugopress/modules/seo/open-graph` | [Open Graph](https://ogp.me/).
| `hugopress/modules/seo/schema` | [Schema](https://schema.org/).
| `hugopress/modules/seo/translations` | Localized pages, see [Tell Google about localized versions of your page](https://developers.google.com/search/docs/specialty/international/localized-versions).
| `hugopress/modules/seo/twitter-cards` | [Twitter Card](https://developer.twitter.com/en/docs/twitter-for-websites/cards/overview/abouts-cards).

## Usage

> Skip this section if your theme support [HugoPress](https://github.com/razonyang/hugopress), all partials will be included automatically.

Just include the partials you want.

```go
{{- partial "hugopress/modules/seo/all" . -}}
```
