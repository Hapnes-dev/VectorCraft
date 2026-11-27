# VectorCraft

A web build of [VectorCraft](https://github.com/storytold/vectorcraft), the open-source vector editor by the
ArtCraft team, served from GitHub Pages.

- **Editor:** https://hapnes-dev.github.io/VectorCraft/app/
- **This page:** https://hapnes-dev.github.io/VectorCraft/

Currently: VectorCraft 0.24.1.

Everything runs in the browser: nothing opened or drawn in the editor is sent anywhere.

## How this build differs from the official web build

- **Built from the official source** at the release tag.
- **One small change of its own.** An object can be marked to keep its size and rotation. A selection of only such
  objects has no handles, and scaling or rotating a selection that holds one only moves it.
- **The wasm ships gzipped.** GitHub refuses a file of 100 MiB or more, so the wasm is stored as
  `vectorcraft-web-<hash>_bg.wasm.gz`. The page unpacks it as it downloads and starts it only once its SHA-384 is
  the one the page was built with.
- **No ArtCraft name.** VectorCraft's code is MIT OR Apache-2.0, but the ArtCraft name, wordmark and mark are
  trademarks, and
  [docs/brand/LICENSE-brand.txt](https://github.com/storytold/vectorcraft/blob/main/docs/brand/LICENSE-brand.txt)
  asks a published modified version to carry none of them. Help › About keeps the attribution.

## Licences

VectorCraft is © the ArtCraft Team and the VectorCraft contributors, licensed [MIT](app/LICENSE-MIT) OR
[Apache-2.0](app/LICENSE-APACHE) (see also [NOTICE](app/NOTICE)). The bundled fonts are under the SIL Open Font
License (`app/OFL-*.txt`), and the PDF backend's licences are in [`app/licenses/`](app/licenses).

This build is not made, endorsed or supported by the ArtCraft team, and it carries none of the ArtCraft marks.
