# markdown-viewer

[![Repository](https://img.shields.io/static/v1?&message=github&style=flat&colorA=000000&colorB=000000&label=&logo=github&logoColor=ffffff)](https://github.com/RodrigoHamuy/markdown-viewer)

Renders Markdown passed via URL parameter. Nothing is saved, the content lives entirely in the URL.

## Usage

Append URL-encoded Markdown as the `md` parameter:

```
https://rodrigohamuy.github.io/markdown-viewer/?md=%23%20Hello
```

Or load Markdown directly on this page:

<label for="md-file-input" style="display:block;cursor:pointer;">
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 600 220" width="100%" style="max-width:600px;display:block;margin:1em auto;" role="img" aria-label="Load a .md file, or paste with Ctrl+V">
  <rect x="10" y="10" width="580" height="200" rx="14" ry="14"
        fill="none" stroke="currentColor" stroke-width="2"
        stroke-dasharray="10 8" opacity="0.55"/>
  <g transform="translate(255 50)" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round" opacity="0.85">
    <path d="M12 4 h44 l24 24 v54 a6 6 0 0 1 -6 6 h-62 a6 6 0 0 1 -6 -6 v-72 a6 6 0 0 1 6 -6 z"/>
    <path d="M56 4 v24 h24"/>
    <text x="45" y="60" text-anchor="middle" font-family="ui-monospace,Menlo,monospace" font-size="14" font-weight="700" stroke="none" fill="currentColor">.md</text>
  </g>
  <text x="300" y="170" text-anchor="middle" font-family="Arial,sans-serif" font-size="24" font-weight="600" fill="currentColor" opacity="0.85">
    Load a .md file
  </text>
  <text x="300" y="198" text-anchor="middle" font-family="Arial,sans-serif" font-size="20" fill="currentColor" opacity="0.65">
    or paste with Ctrl+V / Cmd+V
  </text>
</svg>
</label>
<input id="md-file-input" type="file" accept=".md,.markdown,.mdown,.mkd,.txt,text/markdown,text/plain" style="position:absolute;left:-9999px;width:1px;height:1px;opacity:0;">

<div style="text-align:center;margin:1em auto;">
  <button id="paste-button" type="button" style="font:inherit;padding:0.6em 1.2em;border:1px solid currentColor;border-radius:8px;background:transparent;color:inherit;cursor:pointer;opacity:0.85;">Paste from clipboard</button>
</div>

Longer content is automatically gzipped and base64url-encoded into the `mdz` parameter to fit more into the URL.

Fork of [Kitware/markdown-viewer](https://github.com/Kitware/markdown-viewer).
