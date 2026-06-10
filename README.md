# Pixelnetica Document Scanning SDK for iOS

Document scanner SDK for iOS: document detection, image processing and enhancement, OCR, and PDF/TIFF/PNG output, distributed as a Swift Package with prebuilt binary xcframeworks.

## Products

| Product | Contents |
| --- | --- |
| `DocScanningSDK` | Core SDK — detection, processing, OCR, writers (`import DocScanningSDK`) |
| `DocScanningSDK-UI` | Ready-made UI components (camera screen, page-crop editor, OCR editor) on top of the core (`import DocScanningSDK_UI`). Includes the core framework. |

Most apps want `DocScanningSDK-UI`; choose `DocScanningSDK` alone for a fully custom UI.

## Requirements

- iOS 16.3+
- Swift 5.9+ / Xcode 15+

## Installation

In Xcode: File > Add Package Dependencies, enter

```
https://github.com/Pixelnetica/DocScanningSDK-iOS
```

and add the product(s) you need to your app target.

Or in `Package.swift`:

```swift
dependencies: [
    .package(url: "https://github.com/Pixelnetica/DocScanningSDK-iOS.git", from: "3.1.2-beta.1"),
],
```

The binary xcframeworks (with bundled dSYMs) are attached to the matching [GitHub Release](https://github.com/Pixelnetica/DocScanningSDK-iOS/releases) and are fetched automatically by SwiftPM with checksum verification.

## License key

The SDK requires a Pixelnetica license key at runtime. Request an evaluation or commercial key at [pixelnetica.com](https://www.pixelnetica.com/products/document-scanning-sdk/). Third-party attribution notices ship inside the frameworks.

## Demo

The EasyScanner demo application shows the full integration (camera, editing, OCR, export).

## Support

- Product page: <https://www.pixelnetica.com/products/document-scanning-sdk/>
- Contact: <https://www.pixelnetica.com/contacts.html>
