# Document Scanner Competitor Research

**Research date:** September 6, 2026  
**Scope:** Product capabilities relevant to automatic document-photo cleanup, batch workflows, browser access, and scan quality.  
**Evidence label:** Official product/help pages unless explicitly marked otherwise.

## Executive conclusion

Automatic edge detection, perspective correction, and multi-page scanning are established category features. Adobe Scan, CamScanner, Genius Scan, iScanner, Apple Notes, and Google Drive all provide some combination of them. Several browser tools also provide automatic edge detection and multi-page PDF creation.

Web Document Scanner differentiates itself through a focused combination:

> A browser-first scanner for batches of existing document photos, with automatic page flattening and shadow cleanup as the default path.

Feature lists show what each product offers; the
[same-image comparison](../benchmark/COMPARISON.md) shows how selected products
handle identical difficult photos.

## Product comparison

| Product | Verified strengths | Relevant constraint or difference | Source |
| --- | --- | --- | --- |
| Adobe Scan | Live edge detection, auto crop, image cleaning, AI straightening/curvature correction, imported photos, High-Speed Scan | Requires mobile app; scans save to Adobe cloud; provides review/edit controls | [Adobe Scan documentation](https://www.adobe.com/devnet-docs/adobescan/android/en/scan.html) |
| CamScanner | Batch Scan, automatic page-edge detection, crop, perspective correction, enhancement, shadow cleanup, OCR | App-centered workflow; crop/filter review remains available | [CamScanner product article](https://blog.camscanner.com/2026/07/24/independent-retailer-month-2026-smarter-document-management-for-small-businesses-with-camscanner/) |
| Genius Scan | Document detection, background removal, distortion correction, shadow removal, batch scanning | Requires iOS/Android app; its privacy advantage includes on-device processing | [Google Play product page](https://play.google.com/store/apps/details?id=com.thegrizzlylabs.geniusscan.free), [Genius Scan SDK features](https://geniusscansdk.com/features) |
| iScanner | Automatic cropping, skew/curve correction, background cleanup, multi-page editing and OCR | Requires iOS/Android app for scanning; broad editor/manager workflow | [iScanner official site](https://iscanner.com/), [App Store page](https://apps.apple.com/us/app/iscanner-pdf-document-scanner/id1040093707) |
| Apple Notes | Automatic boundary detection/capture and additional pages saved into one PDF | iPhone/iPad ecosystem; centered on live camera capture in Notes | [Apple iPhone User Guide](https://support.apple.com/guide/iphone/scan-text-and-documents-iph653f28965/ios) |
| Google Drive | Auto capture, crop/rotate, filters, cleanup, additional pages and searchable PDFs | Scanner is available in the mobile app, not Google Drive web; saves into Drive | [Google Drive Help](https://support.google.com/drive/answer/3145835) |
| Microsoft Lens | Historically a major alternative | Retired in 2026; new scans stopped after March 9, 2026. Microsoft recommends OneDrive, which does not save scans locally | [Microsoft support notice](https://support.microsoft.com/en-US/lens/retirement-of-microsoft-lens) |
| OnlineCamScanner | Browser access, corner detection, multiple pages and PDF/image download | Official workflow explicitly includes an adjust-and-crop step before further enhancement | [OnlineCamScanner](https://onlinecamscanner.com/) |
| OptiPix Document Scanner | Browser-local processing, automatic edge detection, perspective correction, multi-page PDF | Offers manual four-corner adjustment when detection is imperfect; positions privacy/local processing as its lead | [OptiPix](https://optipix.art/document-scanner) |

## Web Document Scanner strengths

- Runs in a modern browser without installing a scanner app.
- Accepts existing document photos from a phone or computer.
- Processes multiple uploaded images in one job (up to 15 on Pro).
- Automatically detects, flattens, corrects, and cleans pages.
- Focuses on skewed photos, visible desks, and uneven shadows.
- Exports PDF, images, or ZIP.
- Deletes uploaded and generated files within 24 hours.

## Scan-quality comparison

The published comparison focuses on page geometry, background cleanup,
readability, and consistency using the same source images. Across the available
outputs, Web Document Scanner stands out for stable page flattening and clean,
uniform backgrounds, especially on angled and unevenly lit photos.

Results can vary by source image, app version, device, filter, and crop
adjustments. Publishing the original photos beside every output keeps the
comparison transparent and easy to inspect.

## Reproducible scan-quality benchmark

A 10-image visual comparison and its exported evidence are available in
[`../benchmark/COMPARISON.md`](../benchmark/COMPARISON.md). The larger
methodology below describes how the comparison can be expanded across more
document types and capture conditions.

### Test set

Use at least 100 original, previously unseen photos:

- 20 flat printed documents under even light;
- 20 documents shot at strong horizontal/vertical angles;
- 20 documents with desk and hand shadows;
- 15 wrinkled, folded, or curved pages;
- 15 receipts on light and dark backgrounds;
- 10 handwritten homework pages.

Include multiple phone models, resolutions, paper colors, languages, and indoor lighting conditions. Keep the original files unchanged for every product.

### Competitors

At minimum test:

1. Adobe Scan
2. CamScanner
3. Genius Scan
4. iScanner
5. Apple Notes or Google Drive
6. OnlineCamScanner
7. One additional browser-first scanner
8. Web Document Scanner

Use the current public version and its default/automatic enhancement mode. Record version, date, platform, plan, and every non-default setting.

### Output metrics

Measure each page on:

- **Boundary accuracy:** intersection-over-union against a manually labeled page mask.
- **Content retention:** percentage of ground-truth text/content area preserved.
- **Geometry:** average deviation of text baselines from horizontal and page edges from rectangular.
- **Shadow reduction:** luminance variance across known blank paper regions.
- **Readability:** OCR character error rate using one neutral OCR engine on every output.
- **Detail retention:** small-font and thin-stroke preservation.
- **Manual intervention rate:** percentage of pages requiring corner/filter edits.
- **Workflow effort:** taps/clicks and elapsed time from source import to export.
- **Batch consistency:** variation in paper luminance and contrast across one document.

### Blind review

Randomize and anonymize every output. Ask at least five reviewers to score:

1. readability;
2. geometric correctness;
3. background/shadow cleanliness;
4. natural appearance;
5. submit-readiness.

Reviewers must not know which product produced each page. Publish sample size, scoring instructions, raw aggregate scores, confidence intervals, failures, and ties.

### Interpreting comparative results

Comparative findings are most useful when tied to the tested images, product
versions, and evaluation criteria:

- identify the source set and processing date;
- publish the original and processed images;
- record settings and manual adjustments;
- report both strong and difficult examples;
- distinguish visible observations from measured OCR or geometry scores.

For the current set, the visible results support this concise finding:

> “Web Document Scanner delivers notably consistent flattening and background cleanup across the tested angled and unevenly lit document photos.”
