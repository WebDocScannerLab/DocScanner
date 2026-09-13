# Scan Document Photos Online

**[English](./README.md)** · **[中文](./README.zh-CN.md)**

[Web Document Scanner](https://web-doc-scanner.app) is a fully automatic **online document scanner** for turning existing phone photos into clean, flattened scan PDFs. Upload one page or a batch; the service detects the paper, corrects perspective, reduces shadows, and prepares the pages for export—without installing an app or dragging crop corners page by page.

<p align="center">
  <a href="https://web-doc-scanner.app"><img src="https://img.shields.io/badge/Scan%20a%20document-Open%20web%20scanner-2563eb?style=for-the-badge" alt="Open Web Document Scanner"></a>
</p>

<p align="center">
  <a href="https://web-doc-scanner.app">Scan now</a> ·
  <a href="https://web-doc-scanner.app/zh/">中文版</a> ·
  <a href="https://web-doc-scanner.app/pricing">Pricing</a> ·
  <a href="https://web-doc-scanner.app/contact">Enterprise API</a>
</p>

> This is the public product repository for a hosted commercial service. It contains product documentation, not source code or a self-hosted package.

## Why use [Web Document Scanner](https://web-doc-scanner.app)?

### Fully automatic from upload to scan

Most scanner workflows are built around a live camera and an editing screen. [Web Document Scanner](https://web-doc-scanner.app) is built for photos you already have in your camera roll, email, AirDrop, or chat history. Add the files and let the processing pipeline handle:

- page detection and background removal;
- perspective correction for tilted photos;
- page flattening;
- shadow and uneven-light cleanup;
- scan-style contrast enhancement;
- page ordering and export.

Manual rotation and reordering remain available, but dragging four crop corners is not the default workflow.

### Batch processing for existing photos

Upload multiple document photos together instead of capturing and confirming every page individually. Pro accepts up to **15 images in one scan job**. Reorder the pages once, start the job, and export the results as PDF, images, or ZIP.

This workflow is useful when documents have already arrived through WeChat, email, AirDrop, a camera roll, or a shared folder.

### Built for difficult phone photos

[Web Document Scanner](https://web-doc-scanner.app) is designed to do more than place an original JPG inside a PDF. Its processing targets the defects that make phone photos look unprofessional:

- keystone distortion from shooting at an angle;
- dark desks and visible background;
- overhead-light shadows and hotspots;
- gray or uneven paper backgrounds;
- inconsistent pages within the same batch.

The quality goal is a readable, submit-ready page that looks closer to flatbed output than to a cropped camera photo.

In a [same-image comparison](./benchmark/COMPARISON.md) with Adobe Scan,
CamScanner, and iScanner, [Web Document Scanner](https://web-doc-scanner.app) produced consistently strong
page flattening, background cleanup, and batch-to-batch visual consistency
across the available test outputs. The original photos and every result are
published for direct inspection.

## How it compares

| Product | Runs without app install | Imports existing photos | Automatic correction | Batch / multi-page | Typical workflow |
| --- | --- | --- | --- | --- | --- |
| **[Web Document Scanner](https://web-doc-scanner.app)** | Yes, browser | Yes | Page detection, flattening, perspective and shadow cleanup | Yes, up to 15 images on Pro | Upload batch → process automatically → export |
| Adobe Scan | No, mobile app | Yes | Auto crop, cleaning and AI straightening | Yes, High-Speed Scan | Capture/import → review/edit → save to Adobe cloud |
| CamScanner | No, mobile app | Yes | Auto crop, perspective correction and enhancement | Yes | Capture/import → review crop/filter → export |
| iScanner | No, mobile app | Yes | Auto crop, distortion correction and cleanup | Yes | Capture/import → refine/edit → export |

The market already has capable automatic scanners. [Web Document Scanner](https://web-doc-scanner.app)'s positioning is the combination of:

1. **Browser access** on phone or computer.
2. **Batch import of photos already taken**, not only live camera capture.
3. **Automatic processing as the primary path**, not a crop editor.
4. **Flattening and shadow cleanup** aimed at difficult desk photos.
5. **Direct export** to PDF, images, or ZIP.

## How to scan documents online

1. **Upload one or more photos.** Select JPG or PNG files already on your device.
2. **Arrange the pages.** Reorder or rotate them if necessary.
3. **Start the scan.** Page detection, flattening, and cleanup run automatically.
4. **Export the result.** Download a PDF, individual images, or a ZIP archive.

The free plan includes **1 image per day** with a watermark. [Pro](https://web-doc-scanner.app/pricing) removes the daily limit and watermark and supports up to **15 images per job**.

## Scan quality: what “better” means

Scan quality should be measured, not asserted with an absolute slogan. For this product, “better” means:

- more of the true page retained after automatic detection;
- straighter page geometry and text lines;
- less visible background and shadow;
- higher text readability without crushed characters;
- consistent white balance and contrast across a batch;
- fewer pages requiring manual correction;
- fewer total actions before a usable export.

The [published same-image comparison](./benchmark/COMPARISON.md) highlights
[Web Document Scanner](https://web-doc-scanner.app)'s consistent page geometry and clean backgrounds on
angled, unevenly lit document photos:

> **Cleaner, flatter document scans from difficult phone photos—processed automatically in batches, directly in your browser.**

## Common use cases

- [Homework photos to one PDF](https://web-doc-scanner.app/scan-homework)
- [Receipt and invoice scans](https://web-doc-scanner.app/scan-receipt)
- [Photo to scanned document](https://web-doc-scanner.app/photo-to-scanned-document)
- [JPG or PNG to scanned PDF](https://web-doc-scanner.app/image-to-scanned-pdf)
- [Online image scanner](https://web-doc-scanner.app/online-image-scanner)
- Enterprise document-scanning API

## Product features

- Fully automatic page detection and enhancement
- Batch upload and page reordering
- Perspective correction and page flattening
- Shadow and uneven-background cleanup
- PDF, image, and ZIP export
- English and Simplified Chinese interfaces
- Google sign-in
- Enterprise API access
- Automatic deletion of uploads and generated scans within 24 hours

The current product creates scan images and PDFs. It does not provide OCR or spreadsheet extraction.

## Privacy

Uploaded photos and generated scans are deleted automatically within **24 hours**. We do not sell uploaded documents or use them for advertising. Payments are handled by Stripe, and sign-in uses Google OAuth.

Read the [Privacy Policy](https://web-doc-scanner.app/privacy-policy) and [Terms of Service](https://web-doc-scanner.app/terms-of-service).

## Frequently asked questions

### Do I need to install an app?

No. Open [web-doc-scanner.app](https://web-doc-scanner.app) in a modern browser on a phone or computer.

### Do I need to drag four crop corners?

No. Automatic page detection and correction are the default workflow. You can still rotate and reorder pages when needed.

### Can I upload multiple photos at once?

Yes. Pro supports up to 15 images in one scan job. Add the photos, order them, and process the batch.

### Is this the same as JPG to PDF?

No. A basic converter wraps the original photo in a PDF. [Web Document Scanner](https://web-doc-scanner.app) first detects and flattens the page and cleans the image.

### Is the output always better than every scanner app?

Results vary with document shape, lighting, camera quality, blur, and occlusion. In the published test set, [Web Document Scanner](https://web-doc-scanner.app) stands out for automatic page flattening, background cleanup, and consistent output across difficult angled photos. Review the [same-image results](./benchmark/COMPARISON.md) directly.

### Is an API available?

Yes. [Contact us](https://web-doc-scanner.app/contact) for Enterprise API volume, rate limits, support, and invoice billing.

## Start scanning

[Scan document photos online →](https://web-doc-scanner.app)

[打开中文扫描页 →](https://web-doc-scanner.app/zh/)

---

**[Web Document Scanner](https://web-doc-scanner.app)** · [web-doc-scanner.app](https://web-doc-scanner.app) 
