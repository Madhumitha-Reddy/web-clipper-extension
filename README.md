Web Clipper helps you highlight, capture, and organize web content directly from your browser. Save important information, annotate content, and access your saved clips whenever needed.

## Get started

Install the extension by loading it into your browser in developer mode.

## Use the extension

The extension supports:

* Highlighting content
* Saving web pages and articles
* Custom templates
* Variables and filters
* Content organization and management

## Contribute

### Translations

You can help translate Web Clipper into your language. Submit your translation via pull request using the format found in the [/_locales](/src/_locales) folder.

### Features and bug fixes

Contributions are welcome through pull requests and issue reports.

## Roadmap

In no particular order:

* [ ] Annotate highlights
* [ ] Template directory
* [ ] Sync settings across browsers
* [x] A separate icon for Web Clipper (1.6.3)
* [x] Template validation (1.1.0)
* [x] Template logic (if/for) (1.1.0)
* [x] Save images locally
* [x] Translate UI into more languages

## Developers

To build the extension:

```bash
npm run build
```

This will create three directories:

* `dist/` for the Chromium version
* `dist_firefox/` for the Firefox version
* `dist_safari/` for the Safari version

### Install the extension locally

For Chromium browsers:

1. Open your browser and navigate to `chrome://extensions`
2. Enable **Developer mode**
3. Click **Load unpacked** and select the `dist` directory

For Firefox:

1. Open Firefox and navigate to `about:debugging#/runtime/this-firefox`
2. Click **Load Temporary Add-on**
3. Navigate to the `dist_firefox` directory and select the `manifest.json` file

### Run tests

```bash
npm test
```

Or run in watch mode during development:

```bash
npm run test:watch
```

## Third-party libraries

* webextension-polyfill for browser compatibility
* defuddle for content extraction and Markdown conversion
* dayjs for date parsing and formatting
* lz-string to compress templates and reduce storage space
* lucide for icons
* dompurify for sanitizing HTML

## License

This project is licensed under the MIT License.

