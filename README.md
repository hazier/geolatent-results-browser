# GeoLatent Results Browser

A public, static explorer for 7,762 spatial-reasoning evaluation cases.

| Dataset | Cases | GeoLatent SFT | GeoLatent + RL |
| --- | ---: | ---: | ---: |
| MindCube TinyBench | 1,050 | 761 / 1,050 | 810 / 1,050 |
| MMSI | 1,000 | 321 / 1,000 | 356 / 1,000 |
| ViewSpatial | 5,712 | 2,667 / 5,712 | 2,598 / 5,712 |

Browse questions, answer choices, ground truth, SFT predictions, raw outputs,
and saved latent execution summaries. Filter by category, correctness,
completion, and difficulty. Individual cases and filtered summaries can be
downloaded as JSON and CSV.

RL aggregate results are included. RL per-question predictions will be added
when the corresponding files are available. SFT or historical RL responses are
not used as substitutes.

The site includes all 7,665 unique display images. These hosted WebP copies
preserve the full image and aspect ratio, use a maximum edge of 768 pixels and
quality 84, and have embedded metadata removed. Images load from the public
site, without access to any local drive or research server.

See `data/provenance.json`, `data/summary.json`, and `data/image-manifest.json`
for provenance and source/display image hashes. Dataset and source image
rights remain with their respective authors. This repository does not grant
additional rights to the underlying datasets.

## Hosting

GitHub Pages serves `main` at the repository root. `.nojekyll` preserves this
buildless static layout. All paths are relative, including dataset and image
URLs. The original research and paper repository remains separate and private.

For a local preview, serve this directory with a static HTTP server.
