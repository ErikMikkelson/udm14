# &udm=14 | AI-Free Google Search

A secure, privacy-focused Google search interface that avoids AI-generated overviews and uses only local resources. No external CDNs, trackers, or analytics.

## Features

- **AI-overview-free Google search**: Uses `udm=14` to disable AI summaries.
- **Security-first**: Strict Content Security Policy (CSP), input validation, and CSRF protection.
- **Privacy-focused**: No external scripts, no tracking, no analytics.
- **Dark mode support**: Responsive design with custom dark mode styles.
- **Minimal Tailwind CSS**: Optionally use a purged Tailwind build for only the classes you use.

## Usage

1. Open `index.html` in your browser.
2. Enter your search query and submit. The form securely redirects to Google Search with `udm=14`.

## Security Details

- **CSP**: Only local scripts/styles, strict rules for fonts/images.
- **Form validation**: Prevents HTML injection and enforces query length.
- **CSRF token**: Simple token generated on page load.

## Minimal Tailwind CSS Setup

1. Build the minimal CSS:

```sh
npx tailwindcss -c tailwind.config.js -i ./tailwind-min.css -o ./assets/css/tailwind-min.css --minify
```

## Folder Structure

```text
index.html
assets/
  css/
    style.css
    tailwind-min.css
package.json
tailwind-min.css
tailwind.config.js
README.md
```
