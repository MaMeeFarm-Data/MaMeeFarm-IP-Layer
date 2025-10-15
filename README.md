<div align="center">
  <img src="https://raw.githubusercontent.com/MaMeeFarm-Data/branding/main/logo.png" width="120" alt="MaMeeFarm Logo"/>

  # 🌾 MaMeeFarm™ — Proof-of-Work Farm Data Architecture
  **From Real Labor to Verified Digital Existence**

  [![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC--BY--NC_4.0-green.svg)](LICENSE)
  [![Build Manifest](https://github.com/MaMeeFarm-Data/MaMeeFarm-Data-Metadata/actions/workflows/build_manifest.yml/badge.svg)](https://github.com/MaMeeFarm-Data/MaMeeFarm-Data-Metadata/actions/workflows/build_manifest.yml)
  [![OpenSea Sync](https://github.com/MaMeeFarm-Data/MaMeeFarm-Data-Metadata/actions/workflows/opensea_sync.yml/badge.svg)](https://github.com/MaMeeFarm-Data/MaMeeFarm-Data-Metadata/actions/workflows/opensea_sync.yml)

  > “We do not create synthetic data — we preserve real life.”  
  — MaMeeFarm™ Digital Assets, Lampang Thailand
</div>

---

## 🧭 Overview

**MaMeeFarm-Data-Metadata** is the official data repository of  
**MaMeeFarm™**, the world’s first **Proof-of-Work Farm Data Architecture** —  
a system that transforms real-world labor into verifiable digital records  
on the blockchain.

This repository automatically synchronizes on-chain metadata from  
the [MaMeeFarm OpenSea Collection](https://opensea.io/collection/mameefarm)  
and stores verified JSON snapshots under `/data`.

Each record is a cryptographic “proof of work” that connects  
the physical act of farming with digital asset ownership.

---

## ⚙️ System Structure

```bash
MaMeeFarm-Data-Metadata/
├── LICENSE                   # Creative Commons License
├── TRADEMARK.md               # MaMeeFarm™ trademark declaration
├── DATA-PROVENANCE.md         # Proof-of-Work Data provenance
├── MANIFEST.json              # List of verified files and hashes
├── MANIFEST.SIGN              # Digital signature of manifest
├── fetch_opensea_metadata.py  # Metadata sync script
├── data/                      # Auto-generated NFT metadata
└── .github/workflows/
    ├── opensea_sync.yml       # Daily OpenSea → GitHub sync
    ├── build_manifest.yml     # Manifest auto-verification
    ├── scan_structure.yml     # Anti-copy detection
    ├── alert_fork.yml         # Alert on fork events
    └── alert_star.yml         # Alert on star events
