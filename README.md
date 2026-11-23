<p align="center">
  <img src="android-chrome-512x512.png" alt="Country Code's monogram" width="180" />
</p>

<h1 align="center">Country Code's</h1>

<p align="center">
  An international dialing code reference, grouped by continent.<br />
  Search 214 listings covering shared country codes and non-geographic services.
</p>

<p align="center">
  <a href="LICENSE"><img alt="MIT license" src="https://img.shields.io/badge/license-MIT-2E8B57?style=for-the-badge" /></a>
  <img alt="HTML, CSS, and JavaScript" src="https://img.shields.io/badge/built%20with-HTML%20%2B%20CSS%20%2B%20JS-E34F26?style=for-the-badge" />
  <img alt="214 listings" src="https://img.shields.io/badge/listings-214-0A7EA4?style=for-the-badge" />
  <img alt="6 continents" src="https://img.shields.io/badge/continents-6-8FB840?style=for-the-badge" />
</p>

---

Country Code's is a small, dependency-free reference site for international telephone calling codes. It organizes entries by continent and notes when a code is shared or used for a non-geographic service.

## Features

- Search by country or territory name, or by calling-code digits.
- Filter entries by continent.
- See shared-code notes and non-geographic assignments at a glance.
- Responsive layout with no build step, framework, or runtime dependency.

## Quick Start

Clone the repository and open `index.html` in a browser. The page loads `data.js` from the same directory, so keep both files together.

To serve it locally instead:

```bash
git clone https://github.com/xodo2fast4u/xo-country-codes.git
cd xo-country-codes
python3 -m http.server 8000
```

Then visit [http://localhost:8000](http://localhost:8000).

## Data Notes

The reference follows the international numbering-plan framing of ITU-T Recommendation E.164 and cites ITU Operational Bulletins. The site identifies its data as last updated on **2 September 2026**.

Calling-code assignments do not always map one-to-one to countries. Some codes are shared and need national or area-code context to identify a destination; some entries represent international services rather than geographic countries. Search and continent filters apply to the entries as listed in the dataset.

## Project Files

| File                                                       | Purpose                                                              |
| ---------------------------------------------------------- | -------------------------------------------------------------------- |
| [`index.html`](index.html)                                 | Page layout, styling, search, continent filters, and rendering logic |
| [`data.js`](data.js)                                       | Calling-code records and continent names                             |
| [`site.webmanifest`](site.webmanifest)                     | Web app display and icon metadata                                    |
| `android-chrome-*.png`, `apple-touch-icon.png`, `favicon*` | App icons and browser favicons                                       |
| [`LICENSE`](LICENSE)                                       | MIT license                                                          |

## Development

There is no install or build step. Edit `data.js` to update the reference entries, or `index.html` to change the interface. Check changes by opening the page locally and trying a country search, a code search, each continent filter, and a query with no matches.

When changing records, preserve the `code`, `continent`, and `countries` fields. An optional `note` explains special routing details, and `nonGeo: true` marks an international service rather than a geographic assignment.

## Sources and Disclaimer

The page lists ITU-T Recommendation E.164 and ITU Operational Bulletins as its sources. Telephone numbering assignments can change; consult current official numbering information when accuracy is critical. This project is an independent reference and is not an official ITU publication.

## License

This project is available under the [MIT License](LICENSE).
