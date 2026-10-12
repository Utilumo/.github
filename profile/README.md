# Utilumo

**Browser tools that run on your device.**

Utilumo is a set of browser tools for the small jobs that come up while you work:
converting an image, formatting JSON, splitting a PDF, checking a robots.txt rule.
Files are processed in your browser and never uploaded — the site is a static
export with no backend that could receive them.

→ **https://utilumo.com**

## Browser extension

Clean a link, format selected JSON, tidy copied text, redact a screenshot —
without leaving the page you are on.

- [Chrome Web Store](https://chromewebstore.google.com/detail/utilumo/cfjolblnehaildmonkhdfflnaelmbkad)
- [Edge Add-ons](https://microsoftedge.microsoft.com/addons/detail/utilumo/ennomdcmimeempbcjfpdpeeclknpjdpa)
- [Firefox Add-ons](https://addons.mozilla.org/firefox/addon/utilumo/)

## The ones that are hard to do without a server

| Tool | What it does |
|---|---|
| [Song Analyzer](https://utilumo.com/audio/song-analyzer) | BPM, musical key and Camelot notation — onset envelope, autocorrelation tempo, chroma key detection |
| [Video Compressor](https://utilumo.com/video/video-compressor) | Re-encode video with WebCodecs, in the tab |
| [Split Video](https://utilumo.com/video/split-video) | Cut a video into MP4 segments and download them as a ZIP |
| [SQLite Playground](https://utilumo.com/developer/sqlite-playground) | A real SQLite engine in the browser — tables, seed rows, queries |
| [Audio Merge](https://utilumo.com/audio/audio-merge) | Concatenate several audio files into one WAV |

## Things a generic tool site will not have

| Tool | What it does |
|---|---|
| [Invisible Character Inspector](https://utilumo.com/text/invisible-character-inspector) | Hidden Unicode with names, code points, counts and positions |
| [Compress Image to Size](https://utilumo.com/image/compress-image-to-size) | Hit an exact KB or MB target instead of guessing with a quality slider |
| [Visual Image Diff](https://utilumo.com/image/visual-image-diff) | Slider, onion overlay, side-by-side and pixel-difference views |
| [QR Code Reader](https://utilumo.com/creator/qr-code-reader) | Decode from an image and see the real hostname before opening it |
| [robots.txt Tester](https://utilumo.com/developer/robots-txt-tester) | Which rule actually matches a URL |
| [Prompt Injection Scanner](https://utilumo.com/ai/prompt-injection-scanner) | Overrides, hidden instructions and exfiltration signals |

## Batch, without an account

No sign-up, no queue, no "one file free":

| | Per batch | Total |
|---|---|---|
| Images (resize, convert, EXIF) | 50 files | 500 MB |
| PDFs (merge, split, rotate, compress) | 25 files | 500 MB |
| Audio (MP3 / WAV / FLAC) | 10 files | 500 MB |
| Video | 10 files | 1 GB |

These limits are generous for the same reason nothing is uploaded: there is no
server to pay for. No bandwidth bill, no queue, nothing to police with an account.

## Standards and security

| Tool | What it does |
|---|---|
| [CSP Analyzer](https://utilumo.com/developer/csp-analyzer) | Flag risky directives, copy a hardened starter policy |
| [Security Headers Generator](https://utilumo.com/developer/security-headers-generator) | Build a header set without pasting your domain into a scanner |
| [security.txt Generator](https://utilumo.com/developer/security-txt-generator) | Build a valid RFC 9116 security.txt |
| [security.txt field reference](https://utilumo.com/reference/security-txt-fields) | Every field, with examples |
| [robots.txt directives reference](https://utilumo.com/reference/robots-txt-directives) | Directives and precedence |

## Open data

[Browser tool privacy snapshot](https://utilumo.com/research/browser-tool-privacy-snapshot)
— dataset, methodology and CSV / JSON downloads. Free to cite and re-use.

## What "local" means here, precisely

Your files are processed in the browser and never uploaded to Utilumo. That is a
property of how the site is built, not a policy: it is a static export with no
backend.

Two things do use the network, and neither sends your data to us:

- **Audio conversion** uses encoders bundled with the site, and falls back to an
  ffmpeg WASM build fetched from a CDN when a browser's own codec support is not
  enough. Your media still never leaves the tab.
- **The REST request tester** sends the request you build to the URL you choose.
  That is the whole point of the tool, and it goes straight there, never through us.

Each tool page carries its own privacy note. The
[Privacy Policy](https://utilumo.com/privacy-policy) is the authoritative version.
