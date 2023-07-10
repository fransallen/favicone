<div align="center">
  <img src="icon.svg" width="64" height="64" alt="Favicone logo">
  <h1>Favicone</h1>
  <p>A user-friendly API to get favicons quickly and easily from any website.</p>
  <hr>
</div>

## Example

Get the favicon of a domain:

- https://favicone.com/google.com

Result: ![https://favicone.com/google.com](https://favicone.com/google.com)

Image resizing is available using the **?s=:size** parameter (max is 256):

- https://favicone.com/google.com?s=32

Result: ![https://favicone.com/google.com?s=16](https://favicone.com/google.com?s=16) ![https://favicone.com/google.com?s=32](https://favicone.com/google.com?s=32)

Return the JSON data with **?json** parameter:

- https://favicone.com/google.com?json

```json
{
  "hasIcon": true,
  "icon": "https://icons.favicone.com/i/www.google.com/favicon.ico",
  "format": "ico"
}
```

## About

Favicone is a super convenient API service that allows you to easily retrieve and serve favicons from any website. With its user-friendly URL structure, Favicone makes the process a piece of cake – just use something like `https://favicone.com/:domain`.

The magic happens behind the scenes as Favicone cleverly searches for the favicon link within the website's HTML or directly from the favicon.ico file. It's all about efficiency and simplicity!

You can use Favicone in your app or website to enhance the visual appeal of your app and ensure your users enjoy a seamless favicon experience.

## Used by

The following projects are already using Favicone:

- [Indiwtf](https://indiwtf.upset.dev/monitoring)

If you are using Favicone for your application or website, we invite you to contribute by sending a pull request to add your app/website to the list of users. We would love to showcase how Favicone is being utilized in different projects!

## The Problems

Obtaining a favicon from a website can be a challenging task due to the inconsistent locations where the favicon.ico file or favicon references may be found. The following are common sources where a favicon can be located:

1. favicon.ico file: Traditionally, websites have placed the favicon.ico file at the root directory of the website. However, this is not always the case, and the favicon.ico file may be located in different directories or have a different file name.

2. HTML code: Websites often define a favicon link in their HTML code using the `<link>` tag with the `rel="icon"` attribute. The `href` attribute specifies the URL of the favicon. However, the favicon link can have different variations, such as `rel="shortcut icon"`, `rel="apple-touch-icon"`, or other custom variations.

3. Web manifest file: Modern websites using progressive web app (PWA) technologies may define a web manifest file (manifest.json) that includes information about the website's icons, including the favicon. The web manifest file can specify different sizes and formats for the icons.

These variations in favicon locations and references make it challenging to reliably fetch the favicon for a given website. Favicone aims to address these challenges by searching for the favicon in multiple sources, including the favicon.ico file, HTML code, and web manifest files.

## Similar Services

- [DuckDuckGo Favicons API](https://duckduckgo.com/duckduckgo-help-pages/privacy/favicons/)
- [Google Favicons API](https://www.google.com/search?q=Google+Favicons+API)
