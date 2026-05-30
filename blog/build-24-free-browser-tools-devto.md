# I Built 24 Free Browser Tools That Run 100% Client-Side — No Upload, No Tracking

*Published: June 2026*

Six weeks ago, I started building browser-based tools as a side project. Today, I have **24 tools** — and they've collectively handled zero server requests. Because there is no server.

Every tool is a single HTML file with vanilla JavaScript. Hosted on GitHub Pages. No frameworks, no build step, no backend, no database.

**Hub page:** https://xueboyang1985.github.io/free-browser-tools/

## The Stack

- **Hosting:** GitHub Pages (free, global CDN)
- **Frontend:** Vanilla HTML/CSS/JS — no build tools, no frameworks
- **PDF:** pdf-lib, jsPDF, pdf.js (CDN-loaded)
- **QR:** qrcodejs
- **Images:** Canvas API (built into browser)
- **Crypto:** Web Crypto API
- **State:** localStorage (with try-catch guard)

That's the entire "stack." No backend, no containers, no CI/CD, no database.

## Why Client-Side?

Most "free online tools" make you upload files to their server. With client-side tools:

- Your data never leaves your computer
- No tracking possible (no backend to track you)
- Works offline after first load
- No speed limit from uploads

## The 24 Tools

### PDF Tools (7-in-1)
Merge, split, images↔PDF, extract images, base64, text-to-image. Uses pdf-lib for PDF manipulation. Free limit: 125 pages.

### Image Compressor
Canvas API re-encodes images at adjustable quality. JPG, PNG, WebP. 5MB free limit.

### Image Resizer & Cropper
Canvas API with aspect ratio lock. Touch-friendly crop selector.

### Background Remover
Runs a neural network entirely in-browser via WebAssembly (ONNX runtime). No API key needed. ~5s per image, completely offline.

### Password Generator
crypto.getRandomValues for secure randomness. Adjustable length, character sets, exclude ambiguous chars.

### QR Code Generator
URLs, WiFi, email, SMS, vCard. Wraps qrcodejs.

### JSON-CSV Converter
Bidirectional with bigint support, nested object flattening, smart type inference.

### Base64 Encoder
Text + file encoding, string/hex/binary converter.

### Color Picker
EyeDropper API, color wheel, HEX/RGB/HSL conversion.

### HTML Formatter & CSS Minifier
Tag-aware indentation, whitespace stripping.

### URL Encoder
Full URL and component encoding/decoding + data URL handling.

### Timestamp Converter
Unix seconds, milliseconds, ISO 8601, relative time, timezone-aware.

### Number Base Converter
Binary, octal, decimal, hex. Fractions + step-by-step mode.

### Random Generator
Numbers, coin flip, dice, list picker, shuffle. crypto.getRandomValues.

### Text Diff Checker
Line/char diff with LCS algorithm. Highlighted insertions/deletions.

### Word Counter
Words, chars, sentences, paragraphs, reading time.

### Case Converter
UPPER, lower, Title, Sentence, camelCase, snake_case, kebab-case.

### Markdown Editor
Split-pane with live preview. GitHub-flavored markdown.

### UUID Generator
v4 and v7. Bulk up to 1000. crypto.getRandomValues.

### WhatsApp Chat Formatter
Parse WhatsApp exports → Markdown, HTML, CSV.

### Subtitle Converter
SRT ↔ VTT ↔ ASS. Text extraction mode.

### Kindle Highlights Exporter
Parse My Clippings.txt → Markdown, CSV. Groups by book.

## Monetization

All 24 tools are free. Reasonable free limits (125 PDF pages, 5MB images). The [PRO Bundle ($9.99)](https://xueboyang1985.github.io/free-browser-tools/bundle.html) removes all limits with one license key. One-time payment, lifetime access, 3 devices.

## What I'd Do Differently

1. **Shared component library** — rebuilt toast/modal/PRO badge 24 times
2. **CDN strategy from day one** — deferred loading for heavy libs
3. **SEO upfront** — added blog/sitemap/cross-links retroactively

## The Numbers

24 tools, 6 weeks, zero server costs (GitHub Pages is free). Gumroad takes 9% + $0.30. Revenue so far: $0. Building was easy. Distribution is hard.

## Links

- **Hub:** https://xueboyang1985.github.io/free-browser-tools/
- **PRO Bundle:** https://xueboyang1985.github.io/free-browser-tools/bundle.html
- **GitHub:** https://github.com/xueboyang1985
