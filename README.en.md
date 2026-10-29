# NotebookLM PPT Editor

**Rebuild image-based PDF, PPTX and slide screenshots as PowerPoint slides with editable text.**

[简体中文](README.md) · [Download Mac preview](https://github.com/taomin8879/notebooklm-ppt-editor/releases/download/v0.1.0-build186-public1/NotebookLM-PPT-Editor-0.1.0-build186-public1-macOS-arm64.dmg) · [Release notes](https://github.com/taomin8879/notebooklm-ppt-editor/releases/tag/v0.1.0-build186-public1) · [Feedback](https://github.com/taomin8879/notebooklm-ppt-editor/issues/new/choose)

**Public preview: 0.1.0, build 186 / public1. Apple Silicon only, macOS 13+. LibreOffice is required separately.** This build is ad-hoc signed and **not Apple-notarized**; macOS may block its first launch. The UI and detailed support materials are currently in Chinese.

Independent software; not affiliated with Google or NotebookLM. This repository provides the desktop app and documentation, not its core source code.

## Start here

1. Download the DMG and drag the app into Applications.
2. Install [LibreOffice](https://www.libreoffice.org/download/download-libreoffice/) for rendering and quality checks.
3. Open a PDF, PPTX, PNG or JPG/JPEG. Try one page first in local mode.
4. Inspect the generated PPTX and quality report. Select and edit text in PowerPoint to check the result.

The app includes its runtime, OCR, inpainting models and fonts. Desktop use does not require Python, an API key, a Skill or a first-run model download. Optional DeepSeek enhancement can send extracted text and layout data to the configured service and incur charges.

Recognized text is reconstructed as text boxes; complex artwork may remain as images. Pixel-perfect fidelity, full editability and identical fonts are not guaranteed. A “needs correction” result is not a successful quality acceptance. Check missing text, recognition errors, wrapping, overlaps and numeric values before delivery.

## Installation and verification

[SHA-256 checksums](https://github.com/taomin8879/notebooklm-ppt-editor/releases/download/v0.1.0-build186-public1/SHA256SUMS.txt) verify file integrity, not Apple notarization. Only approve opening software when you trust its source. If macOS reports malware or a damaged file, stop and report the message. Do not disable system-wide security protections.

This preview was checked on the maintainer's Mac; clean-machine installation and arbitrary-document accuracy are not certified. Windows, Intel Mac and Linux builds are unavailable.

## Optional agent integration

[NotebookLM PPT Skill](https://github.com/taomin8879/notebooklm-ppt-skill) calls the separately installed app from a local assistant. It has additional Python and execution requirements and is not needed for desktop use.

Report issues with sanitized examples. Do not post confidential documents or API keys. Contact [tommy_ai@126.com](mailto:tommy_ai@126.com) for private support or licensing. The core app is not open source; public availability does not grant redistribution rights. Third-party components retain their own licenses and notices inside the app.
