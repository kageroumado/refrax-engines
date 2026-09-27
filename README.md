# Refrax engines

Rendering engines for [Refrax](https://github.com/kageroumado/refrax-browser), published as releases of this repository.

- **Releases** named `chromium/<version>-r<revision>` carry `Refrax-Chromium-<version>.zip`, the signed and notarized engine bundle, with its SHA-256, its Ed25519 signature (`.sig`) and the matching dSYMs.
- **The `catalog` release** carries `engines.json`, the list of releases Refrax offers, and `engines.json.sig`.

Refrax installs engines from **Settings → Engines → Available Engines**. It accepts a catalog or an engine only with a valid signature from Refrax's release key, a matching checksum, and Refrax's Developer ID signature on the bundle.

The engine's source is in the Refrax repository: [`Engines/Chromium`](https://github.com/kageroumado/refrax-browser/tree/main/Engines/Chromium), built by [`Scripts/forge`](https://github.com/kageroumado/refrax-browser/tree/main/Scripts/forge) from ungoogled-chromium with Refrax's patches, and the contract every engine implements is [`Engines/CONTRACT.md`](https://github.com/kageroumado/refrax-browser/blob/main/Engines/CONTRACT.md).
