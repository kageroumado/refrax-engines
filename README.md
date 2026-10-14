# Refrax engines

This repository distributes Chromium as an installable rendering engine for [Refrax](https://github.com/kageroumado/refrax-browser). Refrax can switch individual tabs between WebKit and Chromium; this repo holds the engine bundles and update catalog.

Install in Refrax: **Settings → Engines → Available Engines**.

## Highlights

- Add Chromium to Refrax and switch individual tabs between engines.
- Get engine updates through Refrax’s engine catalog.

<details>
<summary>Full feature list</summary>

- Chromium bundles named `Refrax-Chromium-<version>.zip`, released under `chromium/<version>-r<revision>`.
- SHA-256 checksums, Ed25519 signatures, and matching dSYMs.
- The `catalog` release supplies `engines.json` and its signature.
- Refrax checks the catalog signature, bundle checksum, and release-team code signature before installation.

</details>

## Notes

- Requires [Refrax](https://github.com/kageroumado/refrax-browser).
- [Engine source](https://github.com/kageroumado/refrax-browser/tree/main/Engines/Chromium) · [Build tooling](https://github.com/kageroumado/refrax-browser/tree/main/Scripts/forge) · [Engine contract](https://github.com/kageroumado/refrax-browser/blob/main/Engines/CONTRACT.md).
