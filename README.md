<div align="center">

<sup>HMNexus Team</sup>

# 🧬 **HMNexus**
### *A GUI platform for high-speed, code-free TCGA data download*

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.9%2B-blue.svg)](#-technology--language)
[![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20Linux%20%7C%20macOS-lightgrey.svg)](#-installation--quick-start)

🔗 **Project Repository:**  
```bash
https://github.com/your-username/TCGA-DL

🔗 Official TCGA Data Portal (GDC):
https://portal.gdc.cancer.gov/

</div>

🚀 Announcement

We built a Windows app for TCGA downloads!

Downloading TCGA data used to require command-line tools. But my team and I decided to make life easier: we developed a user-friendly graphical interface so researchers can get the data without any coding!

Special thanks to Siamak Salimi, our team lead, for managing the project and guiding the development. 💡


🔗 Download the app here:
https://siamak-salimy.github.io/HMNexus/

This is the kind of teamwork that turns complex tasks into simple solutions!

Overview

TCGA-DL (HMNexus) is a modern, graphical, and high-performance desktop application for downloading The Cancer Genome Atlas (TCGA) data directly from the NCI Genomic Data Commons (GDC) portal.

Developed by the HMNexus Team, HMNexus provides a fully GUI-based, code-free workflow that eliminates the need for command-line tools or scripting, making large-scale cancer genomics data accessible to biologists, clinicians, and researchers without programming experience.

Note

HMNexus is the official project name (previously referred to as TCGADownloader during early development).

Abstract

Background. The Cancer Genome Atlas (TCGA) is a pivotal resource for cancer genomics, yet its utility can be limited for non-programmers because accessing datasets often requires command-line tools or custom scripting. Although the NCI GDC Data Transfer Tool supports manifest-based downloads, it lacks an integrated graphical client and interactive data exploration.

Results. We present HMNexus, an open-source, Tkinter-based desktop application that combines intuitive graphical dataset browsing with high-performance, manifest-driven downloads from the GDC portal. Users can browse and filter TCGA datasets by cancer type, data category (e.g., gene expression, clinical, methylation), and sample attributes using a point-and-click interface, export or import GDC manifest files, and perform optimized concurrent downloads based on those manifests. Benchmarks on an example BRCA cohort (18.2 GB) show download time reductions of up to ~4.8× compared to sequential command-line approaches under typical default settings. Downloaded files are automatically organized into analysis-ready directory structures.

Conclusions. HMNexus bridges the gap between usability and performance, empowering researchers to access TCGA data rapidly and without coding. It is cross-platform, dependency-light (Python 3 + Tkinter), and distributed under the MIT License.

Key Features

✅ Zero coding required — fully graphical, point-and-click interface

⚡ High-speed concurrent downloads via GDC manifest-based parallelism

🧾 Manifest-driven workflow — import/export and consume GDC manifest files as the authoritative file list

📁 Automatic directory organization into analysis-ready folder hierarchies (e.g., BRCA/clinical/, LUAD/rnaseq/)

🔒 MD5 checksum validation for ensuring file integrity after download

🌐 Cross-platform: Windows, macOS, Linux

📦 Standalone executables available (no Python required for end users)

🆓 Open-source under the MIT License


Performance benchmark (example)
|                         Tool | Task                                | Time (18.2 GB BRCA cohort) | Coding Required? |
| ---------------------------: | ----------------------------------- | -------------------------: | :--------------: |
|                  **HMNexus** | Manifest-driven concurrent download |          **12 min 18 sec** |        No        |
|       GDC Data Transfer Tool | Default CLI settings                |              58 min 42 sec |        Yes       |
| TCGAbiolinks (R, sequential) | Single-thread download              |                     54 min |        Yes       |


Note: These benchmark numbers are example results for the specified BRCA cohort. Actual performance varies with network bandwidth, system resources, manifest size, and GDC server behavior / concurrency policies.

How HMNexus works — Technical overview

Dataset selection

Users can browse TCGA projects and metadata inside the GUI, or use the GDC web portal to build complex queries and export a manifest.

Manifest import/export

HMNexus consumes the GDC manifest (a list of file UUIDs and relative paths) as the authoritative download plan.

Parallel download engine

A manifest-driven, multi-process/multi-thread download engine performs concurrent HTTP requests, supports retries, rate/throughput controls, and respects GDC access policies.

Post-download processing

Files are MD5-verified and moved into a clean directory layout suited for downstream bioinformatics pipelines.

Technology & language

Programming language: Python 3.9+

GUI framework: Tkinter

Download engine: Manifest-driven, parallel (multiprocessing / concurrent requests)

Packaging: PyInstaller for standalone executables

License: MIT License

Installation & quick start
Option 1 — Standalone executable (recommended)

Download the appropriate release for your OS from the Releases page and run the executable (no Python required).

Option 2 — Run from source
```bash
git clone https://github.com/your-username/TCGA-DL.git
cd TCGA-DL
pip install -r requirements.txt
python main.py
```

Official GDC portal (for selection & manifest export)
https://portal.gdc.cancer.gov/

### Developers (HMNexus Team)

### Siamak Salimy

## Amirmohammad Asgari

## Mohammadreza Shahbazi

## Abolfazl Ghasemi

## Mahan Mirzade

Usage notes & best practices

Manifest creation: For complex filters (multiple projects, specific sample attributes), we recommend building the manifest in the GDC portal and importing it into HMNexus for download.

Concurrency settings: Adjust the number of concurrent workers according to your network and storage I/O to avoid bottlenecks or GDC throttling.

Data governance: HMNexus does not change file content or access controls; users must comply with GDC data access policies and authorized data usage agreements.

Reproducibility: Use the exported manifest and organized directory layout as part of reproducible analysis pipelines (e.g., store the manifest with your analysis repository).

Acknowledgements

Special thanks to Siamak Salimi, our team lead, for managing the project and guiding the development.
Thanks also to the GDC team for providing portal and API services, and to all contributors and early testers from the HMNexus development group.

Citation

If you use HMNexus in your research, please cite:
Salimy S., Asgari A., Shahbazi M., Ghasemi A., Mirzade M. HMNexus: A GUI Platform for High-Speed, Code-Free TCGA Data Download. BMC Bioinformatics (2025).

## License & contact

This project is released under the MIT License. See LICENSE for full terms.

© 2025 HMNexus Project


Changelog (short)

v1.0.0 — Initial public release: GUI manifest import/export, parallel download engine, MD5 verification, automatic directory organization, standalone executables.

<div align="center"> 🧬 **HMNexus** — *Fast. Simple. Reliable TCGA Data Access.* </div> ```
