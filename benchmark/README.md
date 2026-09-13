# Document Scanner Pilot Benchmark

This directory contains a 10-image visual comparison of [Web Document Scanner](https://web-doc-scanner.app),
Adobe Scan, CamScanner, and iScanner. It focuses on visible differences in page
geometry, background cleanup, readability, and output consistency.

## Contents

- [`COMPARISON.md`](./COMPARISON.md): English side-by-side image comparison.
- [`COMPARISON.zh-CN.md`](./COMPARISON.zh-CN.md): Chinese comparison page.
- `comparison-images/`: scanner outputs placed on identical 900×1100 canvases
  with aspect ratios preserved, so every result displays at the same height.
- `inputs/`: the 10 unchanged JPEG inputs, linked directly without padding.
- `results/`: exported images grouped by product.
- `RESULTS.md` / `RESULTS.zh-CN.md`: coverage and interpretation limits.
- `RESULTS.csv`: per-image output availability.

## Dataset and attribution

The inputs are frames extracted from the official SmartDoc 2015 Challenge 1
sample dataset:

- Source: https://zenodo.org/records/1230218
- DOI: https://doi.org/10.5281/zenodo.1230218
- License: Creative Commons Attribution 4.0 International
- Source archive MD5: `1ee5b7c290d707bd51c59f0b1c1a36f5`

Please cite:

> Jean-Christophe Burie et al., “ICDAR2015 Competition on Smartphone Document
> Capture and OCR (SmartDoc),” ICDAR 2015.

The selected frames cover three document layouts and ten distinct camera
positions with perspective, scale, illumination, glare, and background
variation. They all come from the sample dataset's `background00` scene, so
this pilot does not cover the full range of receipts, handwriting, folds, or
dark backgrounds proposed for the future 100-image benchmark.

## Reproduction rule

Each product received the same JPEG files in filename order. The comparison
uses the supplied exports as evidence; mobile-app versions and processing
settings were not independently audited. iScanner sample 10 remains pending.
See the result reports for product-specific limits.
