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
  "icon": "https://www.google.com/favicon.ico",
  "type": "ico"
}
```

# About

Favicone is a super convenient API service that allows you to easily retrieve and serve favicons from any website. With its user-friendly URL structure, Favicone makes the process a piece of cake – just use something like `https://favicone.com/:domain`.

The magic happens behind the scenes as Favicone cleverly searches for the favicon link within the website's HTML or directly from the favicon.ico file. It's all about efficiency and simplicity!

You can use Favicone in your app or website to enhance the visual appeal of your app and ensure your users enjoy a seamless favicon experience.
