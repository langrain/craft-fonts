# craft-fonts
Font library for ArtCraft

# ArtCraft-FontPack (Unofficial)

An open-source, community-driven font repository designed for **ArtCraft** (especially for `PhotoCraft`). 

This repository aims to solve the **CJK (Chinese, Japanese, Korean) font missing issue** without bloating the main software installer. It provides a lightweight, on-demand font downloader solution for ArtCraft users.

> **中文简介**：这是一个为 ArtCraft 系列软件（特别是 PhotoCraft）打造的开源字体仓库。旨在通过“按需下载”的方式解决中日韩字体缺失问题，同时保持软件本体的极致轻量（不增加安装包体积）。

---

##  Why this repository exists? (为什么要建这个仓库？)

1. **Bloated Installer**: Bundling a single Chinese font (usually 10MB-20MB) will ruin the 190MB lightweight advantage of PhotoCraft.
2. **Licensing Hell**: Many "free" Chinese fonts have strict redistribution restrictions. We only provide 100% open-source fonts (like SIL OFL 1.1) that are safe for commercial use and software redistribution.
3. **Missing Font Fallback**: When opening PSDs with missing fonts, users currently get ugly system fallbacks. This repo provides the resource backend for a smart "Download & Apply" feature.

---

## 🗂️ Repository Structure (仓库结构)

```text
ArtCraft-FontPack/
├── fonts/
│   ├── 851-Handwriting/
│   │   ├── 851ShouShuKIFUONTO-Regular.ttf
│   │   └── LICENSE.txt
│   ├── LXGW-WenKai/
│   │   ├── LXGWWenKai-Regular.ttf
│   │   └── OFL.txt
│   └── Smiley-Sans/
│       ├── SmileySans-Oblique.ttf
│       └── OFL.txt
         ......(other fonts)
├── manifests/
│   └── fonts.json       <-- Used by the software to fetch download URLs
└── README.md
