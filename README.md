[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

# Kidlat Hugo Theme

Kidlat is a low-bandwidth, text-only [Hugo](https://gohugo.io) theme.

This theme is verified to work with Hugo versions v0.110.0–v0.121.2.

![Kidlat screenshot](https://raw.githubusercontent.com/kidlat2024/kidlat/main/images/screenshot.png)

## Features

- Super lightweight
- Responsive layout
- Auto light/dark mode (determined by device's OS setting)
- No framework
- No javascript
- Full-text RSS feed
- [100% score on performance, accessibility, best practices and SEO](https://pagespeed.web.dev/analysis/https-kidl-at/k1i6fc1anh?form_factor=mobile) on PageSpeed Insights

## Example site

This theme is in use at [Kidlat News](https://kidl.at). Our site's [Github repo](https://www.github.com/kidlat2024/kidlatnews/) is public.

## Installation

1. Copy the `kidlat` folder inside the `themes` folder of your site.

```
themes/
└── kidlat
```

2. Add the theme to the [site configuration](https://gohugo.io/getting-started/configuration/) file (`config.yaml`).

```
theme: kidlat
```

## Configuration

### 1. Change the default configuration

Copy and change the default theme configuration inside `hugo.yaml` to the [site configuration](https://gohugo.io/getting-started/configuration/) file `config.yaml`:

```
baseURL: https://example.org/        # Change to your website URL
title: Example News & Current Events # Change to your website title
languageCode: en-us
theme: kidlat

params:
  short_title: Example News           # Change to your website short title
  display_name: EXAMPLE               # Change to your website display name
  license: Creative Commons BY-SA 4.0 # Change to your website license
  license_url: https://creativecommons.org/licenses/by-sa/4.0/deed.en # Change to your license URL
  description: "Example News is the trusted site for news and current events." # Change to your website description
  logo: "/example-news.jpg" # The logo should be inside your static folder
  footer: <span><a href="http://www.example.org/">This is the footer text.</a></span> <span><a href="#top">▲</a></span> # Change to your footer text and link
```

### 2. Put the `css` folder inside your `static` folder

Move or copy the `css` folder and its contents to your site's `static` folder. Your `static` folder should look like this.

```
static/
└── css
   ├── kidlat.css
   └── README.md
```

### 3. Specify items in the front matter

There are a number of optional front matter items that can be specified.

- `content_type` For [schema.org](https://schema.org/) metadata. The most common types are `Article`, `NewsArticle` and `BlogPosting`.

- `attribution` To attribute images to their source and specify their license.

- `display_license` To display the site license (as well as the `attribution` if specified) at the end of each article, set this to `true`. 

- `images` To specify the image metadata. This image will be used when the article is shared on social media.

- `xurl` If shared on Twitter, the URL of the tweet. If the URL is specified, a `Comment on X` appears after the article post date.

## License

Kidlat theme is licensed under the [Apache License 2.0](https://github.com/kidlat2024/kidlat/blob/main/LICENSE).
