<div align="center">

<img src="https://dustystorage.com/images/logo.png" alt="Dusty Logo" width="80" height="80" />

# Dusty — AI-Powered Storage Cleaner for macOS

**Other cleaners find big files. Dusty understands what they are.**

[![macOS 14+](https://img.shields.io/badge/macOS-14.0%2B%20(Sonoma%20%2F%20Sequoia)-000000?style=for-the-badge&logo=apple&logoColor=white)](https://dustystorage.com)
[![Apple Silicon & Intel](https://img.shields.io/badge/Architecture-Universal%20(M1%2FM2%2FM3%2FM4%20%26%20Intel)-FF6F00?style=for-the-badge&logo=apple)](https://dustystorage.com)
[![Swift Native](https://img.shields.io/badge/Built%20With-Swift%20%26%20SwiftUI-F05138?style=for-the-badge&logo=swift&logoColor=white)](https://dustystorage.com)
[![Homebrew](https://img.shields.io/badge/Homebrew-Cask-FBB040?style=for-the-badge&logo=homebrew&logoColor=black)](https://github.com/sarmadhussainch/homebrew-dusty)
[![Privacy](https://img.shields.io/badge/Privacy-100%25%20Local%20Scanning-10B981?style=for-the-badge&logo=shield)](https://dustystorage.com/privacy.html)

<br />

<img src="https://dustystorage.com/images/dusty-app-main-ui.png" alt="Dusty macOS App Main Interface" width="880" />

<br />
<br />

[Website](https://dustystorage.com) • [Features](https://dustystorage.com/features.html) • [AI Flow](https://dustystorage.com/ai-flow.html) • [Pricing](https://dustystorage.com/pricing.html) • [Changelog](https://dustystorage.com/changelog.html)

</div>

---

## ⚡ Quick Install via Homebrew

Install Dusty in one command with zero Gatekeeper security prompts:

```bash
brew install sarmadhussainch/dusty/dusty
```

Or tap first:

```bash
brew tap sarmadhussainch/dusty
brew install --cask dusty
```

> **Direct Download:** Prefer a standalone `.zip` or `.dmg`? Download directly from [dustystorage.com](https://dustystorage.com).

---

## 🎯 Why Dusty?

Traditional Mac cleaners show you confusing lists of obscure file paths and ask you to blindly click *"Clean All"*. You risk deleting active project caches, critical dependencies, or chat history.

**Dusty takes a trust-first approach:**
1. **Understands File Context:** It analyzes what generated the file, why it's there, and whether it can be safely rebuilt.
2. **Plain-English AI Explanations:** Before anything is moved, Dusty explains every cleanup decision in plain English.
3. **Trash-First Safety:** Moves files to macOS Trash instead of permanent deletion, so you can restore anything with one click.
4. **Never-Touch Protection:** System files, Git histories, and chat databases are permanently locked and safeguarded.

---

## ✨ Key Features

### 🛠️ 1. Developer Project Bloat Sweeper
Reclaim 20 GB – 100 GB+ lost to stale developer dependencies and build caches without breaking your repositories:
* **Package Dependencies:** `node_modules`, Composer `vendor`, `.parcel-cache`, `coverage`.
* **Framework Build Outputs:** `.next`, `.nuxt`, `.turbo`, `build`, `dist`, `target` (Rust/Cargo).
* **Safe Rebuilding:** Clear labels indicating which folders can be restored with `npm install`, `pnpm install`, `composer install`, or `cargo build`.
* **Source Protection:** Never touches `.git`, source files, or `.env` configurations.

### 📦 2. One-Click App Uninstaller
Dragging an app to Trash leaves gigabytes of leftover cache, application support files, and containers behind:
* **Deep Residual Discovery:** Scans `~/Library/Application Support`, `Caches`, `Containers`, `Preferences`, and `Logs`.
* **AI Disk Footprint Breakdown:** Explains exactly where the app stored data and what is safe to remove.
* **Complete Removal:** Cleans leftover dependencies in 1-click.

### 💬 3. WhatsApp Desktop Media Cleaner
WhatsApp Desktop stores duplicate copies of videos, voice notes, and high-res photos locally:
* **Media Cache Purge:** Cleans bloated cached attachments and media files.
* **Database Shield:** Strictly protects `ChatStorage.sqlite` and conversation history.

### ⚡ 4. User & Package Manager Caches
* **Browser Caches:** Google Chrome, Brave, Microsoft Edge, Electron caches.
* **Dev Tool Caches:** pip, Composer, ms-playwright, node-gyp, Homebrew, and Gradle caches (`~/.gradle/caches`, `~/.cache`).

### 📥 5. Smart Downloads & Large File Triage
* **Old Installers & Archives:** Surfaces DMGs, ZIPs, TAR/GZ, and APKs older than 45 days.
* **Heavy Untouched Files:** Highlights large media (>100 MB) sitting idle for review before deletion.

---

## 🛡️ Trust-First Risk Categorization

Every detected file is classified into strict trust categories:

| Category | Risk Level | Action | Description |
| :--- | :---: | :---: | :--- |
| **Safe to Delete** | 🟢 Safe | Checked by default | Browser caches, temp logs, and rebuildable thumbnails. |
| **Rebuildable** | 🔵 Rebuildable | Checked by default | `node_modules`, `vendor`, and framework build caches. |
| **Review First** | 🟡 Review | Unchecked by default | Downloads, DMGs, duplicate project folders, and chat media. |
| **Never Touch** | 🔴 Protected | Permanently Locked | System files, Git databases, source code, and chat history. |

---

## 🔒 Privacy & Local Security

* **100% Local Scanning:** Scanning runs entirely on your Mac using native Swift file system actors.
* **Zero File Content Uploads:** Dusty never reads or transmits the contents of your files, source code, or documents.
* **Metadata-Only AI Insights:** When generating AI explanations, Dusty sends only anonymized metadata (file name, path structure, size, and age).
* **Zero Telemetry:** No user tracking, no behavioral analytics.

---

## 💻 Homebrew Commands

### Upgrade to the Latest Version
```bash
brew upgrade --cask dusty
```

### Uninstall Dusty
```bash
brew uninstall --cask dusty
```

### Clean Up All Preferences & Caches
```bash
brew uninstall --zap --cask dusty
```

---

## 📋 System Requirements

* **Operating System:** macOS 14.0 (Sonoma), macOS 15.0 (Sequoia), or later.
* **Architecture:** Universal Binary (Native Apple Silicon M1/M2/M3/M4 + Intel 64-bit).
* **Permissions:** Standard user file permissions (Full Disk Access optional for deep system-wide scans).

---

## 🎁 24-Hour Free Trial

Dusty comes with a **24-Hour Full-Access Free Trial** with no credit card required. Experience full deep scans, AI explanations, and smart disk cleanup immediately upon launch.

* **Website:** [https://dustystorage.com](https://dustystorage.com)
* **Pricing & Licenses:** [https://dustystorage.com/pricing.html](https://dustystorage.com/pricing.html)
* **Support & Contact:** [support@dustystorage.com](mailto:support@dustystorage.com)

---

<div align="center">

Made with care for Mac users and developers worldwide.

© 2026 [Dusty Storage](https://dustystorage.com). All rights reserved.

</div>
