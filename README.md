# VideoSqueezer

![version: v1.7.0](https://img.shields.io/badge/version-v1.7.0-blue?style=plastic&labelColor=555) ![HTML5: single-file](https://img.shields.io/badge/HTML5-single--file-orange?style=plastic&labelColor=555) ![offline: ready](https://img.shields.io/badge/offline-ready-green?style=plastic&labelColor=555) [![License: GPL-3.0-or-later](https://img.shields.io/badge/License-GPL--3.0--or--later-blue?style=plastic&labelColor=555)](LICENSE)

Edit local videos and create animated GIFs in one HTML file.

## Live application:

[https://firerayo.github.io/VideoSqueezer/](https://firerayo.github.io/VideoSqueezer/)

Expected address; HTTP 404 on November 10, 2026. Publication is not confirmed.

## Features

- Add multiple videos with **Add videos** or drag and drop. Select, reorder, or remove inputs.
- **Trim** exports the blue range. **Split** creates two files at its selected point.
- Use millisecond inputs, draggable handles, playhead marks, reset, zoom, and frame stepping. **Preview selection** follows the range.
- **Join** orders full videos. Swap two or select positions. Optional settings enable audio, compression, conversion, and GIF.
- **Rotate:** 90°, 180°, or 270° clockwise. Compatible original copy uses orientation metadata.
- **Keep format · Prefer original:** compatible MP4, MOV, or M4V track copying. Exact cuts can require H.264 encoding.
- **Reduce size · Same format:** MP4, MOV, M4V, or WebM compression, with a 5–90% target and codec policy.
- Source resolution is initially kept. Results show actual savings and must be smaller.
- **Re-encode / Convert** offers supported MP4/H.264 or WebM output, quality presets, 0.2–12 Mbps video bitrate, and frame shapes.
- Choose 480p, 720p, or 1080p and 24, 25, or 30 frames per second (fps). Set 0–100% volume; zero removes audio.
- **Convert to GIF:** 1–100% maximum of the source or range reference. Resolution, frame rate, and colors adapt.
- GIF supports all four operations, without audio, and loops continuously. Impossible size targets are rejected.
- Review duration, size estimates, warnings, and progress. Cancel exports, download individual results, or select **Clear results**.
- Switch English, Spanish, Italian, or Brazilian Portuguese without reloading. Choose light or dark appearance.
- Open **About** for copyright, credits, source, warranty information, and the full offline GNU GPL text.

## Quick start

1. Download and open [index.html](index.html) in a current browser.
2. Add videos under **01 Upload** and choose an operation under **02 Edit**.
3. Review **03 Size**, export, and save results under **04 Download**.

Example: trim a selected range, preview, then export.

No installation, server, or build. Browser codecs determine compatibility.

## Limitations and compatibility

| Limit | Desktop | Mobile |
| --- | --- | --- |
| Per input / combined inputs | 512 / 1,024 MiB | 128 / 256 MiB |
| Per video output / retained results | 512 / 640 MiB | 128 / 192 MiB |
| Video export duration | 20 minutes | 5 minutes |
| GIF duration / per output | 30 seconds / 20 MiB | 15 seconds / 8 MiB |

Both profiles support 10 inputs, 60 minutes per source, and 0.25-second minimum ranges or parts.
Inputs are limited to 4,096 pixels per side and 4,096 × 2,160 pixels total.
Native compression and exact original-container cuts are limited to 1080p.

Original copy requires classic, self-contained sample tables and compatible tracks for joining.
Fragmented, protected, external-reference, or unsupported tracks are blocked. Recognized high dynamic range input blocks re-encoding.

Compression can change quality, timing, and metadata. Copied audio can leave brief silence at cut edges.
GIF uses up to 640 pixels on desktop or 480 on mobile, nominally 12 fps, and up to 256 colors.
Its size percentage is a ceiling; cropped-range references are estimates. GIF timing rounds to 0.01 seconds.
Keep the tab visible during re-encoding or GIF creation. Limits do not guarantee sufficient memory.

## Data and privacy

Videos and results stay in session memory. Originals remain unchanged. Only language and theme preferences use local storage.
Remove inputs or clear results to release references. Save results before closing.
The HTML has no automatic network requests, analytics, remote fonts, or runtime libraries. Repository links require selection; README badges use external images.

## Development and tests

Edit the HTML directly. Configuration, translations, requirements, and history are included.
GIF tests used native Canvas and video fixtures. Independent readers checked pixels, timing, looping, and size limits.
Static checks cover syntax, translations, legal text, and packaging. Browser execution of v1.7.0 remains unverified here.
Earlier Chromium 133 video tests used v1.6.0. Safari, Firefox, touch, and real mobile checks remain pending.

## Contributing and support

Report bugs and propose changes in the [repository](https://github.com/FireRayo/VideoSqueezer). Include reproduction steps and browser details.

## License and credits

Copyright (C) 2026 Raymundo Ortiz. Original application code uses the GNU General Public License,
version 3 or, at your option, any later version published by the Free Software Foundation: **GPL-3.0-or-later**.
See [LICENSE](LICENSE). This program comes without any warranty.

Third-party material retains its original copyright notices and licenses.
The Graphics Interchange Format is the copyright property of CompuServe Incorporated. GIF is a service mark of CompuServe Incorporated.
