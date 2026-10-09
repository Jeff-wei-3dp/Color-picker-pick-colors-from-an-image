# Color Picker for Images: read HEX, RGB and HSL from any photo

A free online colour picker that works on **any image**, right in the browser. Open a photo, click a pixel, and get the exact **HEX**, **RGB** and **HSL** values, plus the dominant colour palette of the whole image.

**Use it here: [allfreekit.com/color-picker](https://www.allfreekit.com/color-picker/)**

No sign-up, no install, no upload. The image is read locally with `<canvas>`, so it never leaves your device.

---

## What it does

| | |
|---|---|
| **Eyedropper on any image** | Load a JPG, PNG, WebP, HEIC, GIF or BMP and click anywhere to read that exact pixel |
| **HEX, RGB and HSL together** | Every format is shown at once, and each value copies with one click |
| **Dominant palette extraction** | Pulls the main colours out of a photo and ranks them by how much of the image they cover |
| **Zoom and magnifier** | Pick precisely on small details instead of guessing at a scaled-down preview |
| **Recent colours** | Keeps the swatches you already picked so you can compare them |
| **Works offline** | After the first visit the page keeps working with no connection |

## How to use it

1. Open **[the color picker](https://www.allfreekit.com/color-picker/)**.
2. Drop an image onto the panel, click to choose a file, or paste a screenshot with `Ctrl+V`.
3. Click any pixel to read its HEX, RGB and HSL values.
4. Copy a value, or export the extracted palette.

<img width="2145" height="1389" alt="pick colors from an image" src="https://github.com/user-attachments/assets/5800b03a-3e71-4234-a33b-5eee5a59500f" />


## Why nothing is uploaded

Most online colour pickers send your image to a server to read the pixels. This one has no server in the path: the file is drawn into a `<canvas>` and sampled locally with JavaScript. That is also why it keeps working offline, why there is no file-size limit, and why you can use it on screenshots of internal designs or client work without a second thought.

## Frequently asked

**Can I pick a colour from a photo on my phone?**
Yes. It works in current Chrome, Edge, Firefox and Safari, including iOS and Android.

**Does it support HEIC from an iPhone?**
Yes. HEIC is decoded in the browser before sampling, so there is no conversion step.

**Can I get a palette instead of a single pixel?**
Yes. Palette extraction groups similar colours and ranks them by coverage, which is what you want when matching a design to a photograph.

**Is there a file-size limit?**
No fixed limit. The practical ceiling is your own device's memory, because the work happens locally.

**Can I use the colours commercially?**
Yes. Colour values are not copyrightable, and nothing is added to your files.

## More free browser tools

All of these work the same way: locally, with no upload and no account.

- **[Remove the background from a photo](https://www.allfreekit.com/remove-background/)** - cut out a subject and download a transparent PNG
- **[Convert an image to Base64](https://www.allfreekit.com/image-to-base64/)** - get a data URI for CSS or HTML
- **[Extract text from an image](https://www.allfreekit.com/image-to-text/)** - OCR that runs in your browser
- **[Resize an image](https://www.allfreekit.com/resize-image/)** - exact pixel dimensions, no upload
- **[Compress an image to 200KB](https://www.allfreekit.com/compress-image-to-200kb/)** - hit an exact file-size limit
- **[Convert HEIC to JPG](https://www.allfreekit.com/heic-to-jpg/)** - iPhone photos, decoded locally

**[All 97 tools on AllFreeKit](https://www.allfreekit.com/)**

## Built with

Plain HTML, CSS and JavaScript. Image reading uses `<canvas>` and `createImageBitmap` where the browser supports it. No framework, no build step, no dependencies.

## Privacy

There is no backend and no analytics in this project. Images you open never leave your device.

## License

MIT.
