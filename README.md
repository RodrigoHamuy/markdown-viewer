# markdown-viewer

[![Repository](https://img.shields.io/static/v1?&message=github&style=flat&colorA=000000&colorB=000000&label=&logo=github&logoColor=ffffff)](https://github.com/RodrigoHamuy/markdown-viewer)

Renders Markdown passed via URL parameter. Nothing is saved, the content lives entirely in the URL.

## Usage

Append URL-encoded Markdown as the `md` parameter:

```
https://rodrigohamuy.github.io/markdown-viewer/?md=%23%20Hello
```

Or paste Markdown directly on this page with `Ctrl+V` / `Cmd+V`.

Longer content is automatically gzipped and base64url-encoded into the `mdz` parameter to fit more into the URL.

Fork of [Kitware/markdown-viewer](https://github.com/Kitware/markdown-viewer).
