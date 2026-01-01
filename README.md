<div align="center">

<sup>HMNexus Team</sup>

# 🧬 **HMNexus (TCGA-DL)**
### *A Tkinter GUI platform for high-speed, code-free TCGA data download*

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.9%2B-blue.svg)](#technology--language)
[![GUI](https://img.shields.io/badge/GUI-Tkinter-blue.svg)](#technology--language)
[![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20Linux%20%7C%20macOS-lightgrey.svg)](#installation--quick-start)

🔗 **Project Page & Download:**  
https://siamak-salimy.github.io/HMNexus/

🔗 **Official TCGA Data Portal (GDC):**  
https://portal.gdc.cancer.gov/

</div>

---

## 🚀 Announcement

We built a **Windows desktop application** for downloading TCGA data.

Accessing TCGA datasets traditionally required command-line tools and scripting.  
The **HMNexus Team** designed this application to eliminate that barrier by providing a **fully graphical Tkinter-based interface**, allowing researchers to download TCGA data **with zero coding**.

Special thanks to **Siamak Salimy**, our team lead, for managing the project and guiding the development. 💡

🔗 Download the application:  
https://siamak-salimy.github.io/HMNexus/

This project demonstrates how teamwork can transform complex bioinformatics workflows into simple, accessible solutions.

---

## Overview

**HMNexus (formerly TCGADownloader)** is a modern, open-source, high-performance desktop application for downloading  
**The Cancer Genome Atlas (TCGA)** data directly from the **NCI Genomic Data Commons (GDC)**.

Developed using **Python + Tkinter**, HMNexus provides a **code-free, GUI-driven workflow** for manifest-based TCGA downloads, making large-scale cancer genomics data accessible to:

- Biologists  
- Clinicians  
- Medical researchers  
- Students and trainees  

without requiring programming expertise.

---

## Project Naming

> **HMNexus** is the official project name.  
> The tool was previously referred to as **TCGADownloader** during early development.

---

## Abstract

**Background**  
The Cancer Genome Atlas (TCGA) is a foundational resource for cancer genomics research. However, downloading TCGA data typically requires command-line tools or scripting, limiting accessibility for non-technical users. While the NCI GDC Data Transfer Tool supports manifest-based downloads, it does not provide a graphical interface or interactive dataset exploration.

**Results**  
We present **HMNexus**, an open-source, Tkinter-based desktop application that integrates intuitive graphical dataset selection with high-speed, manifest-driven downloads from the GDC portal. Users can browse TCGA datasets by cancer type and data category, import or export GDC manifest files, and perform optimized concurrent downloads using a point-and-click interface. Benchmark experiments on a BRCA cohort (18.2 GB) demonstrate up to **4.8× faster** downloads compared to sequential command-line workflows under default settings. Downloaded files are automatically organized into analysis-ready directory structures.

**Conclusions**  
HMNexus bridges the gap between usability and performance, enabling rapid and effortless TCGA data access. The tool is cross-platform, lightweight (Python 3 + Tkinter), and released under the MIT License.

---

## Key Features

- ✅ **Zero coding required** — fully graphical Tkinter interface  
- ⚡ **High-speed concurrent downloads** using GDC manifest files  
- 🧾 **Manifest-driven workflow** — import/export official GDC manifests  
- 📁 **Automatic directory organization** (e.g. `BRCA/clinical/`, `LUAD/rnaseq/`)  
- 🔒 **MD5 checksum validation** for data integrity  
- 🌐 **Cross-platform**: Windows, Linux, macOS  
- 📦 **Standalone executables** available  
- 🆓 **Open-source** under the MIT License  

---

## Performance Benchmark (Example)

| Tool | Interface | Time (18.2 GB BRCA cohort) | Coding Required |
|----|----|----|----|
| **HMNexus** | GUI (Tkinter) | **12 min 18 sec** | No |
| GDC Data Transfer Tool | CLI | 58 min 42 sec | Yes |
| TCGAbiolinks (R) | Scripted | ~54 min | Yes |

> Performance depends on network bandwidth and system resources.

---

## Technology & Language

- **Programming language:** Python 3.9+  
- **GUI framework:** Tkinter  
- **Download engine:** Manifest-based concurrent HTTP downloads  
- **Packaging:** PyInstaller  
- **License:** MIT  

---

## Installation & Quick Start

### Option 1 — Standalone Executable (Recommended)

Download and run the executable for your operating system from:

https://siamak-salimy.github.io/HMNexus/

No Python installation required.

---

### Option 2 — Run from Source

```bash
git clone https://github.com/siamak-salimy/TCGA-DL.git
```
```bash
cd TCGA-DL
```
```bash
pip install -r requirements.txt
```
```bash
python main.py
```

#### Developers — ( HMNexus Team )

### Siamak Salimy

## Amirmohammad Asgari

## Mohammadreza Shahbazi

## Abolfazl Ghasemi

## Mahan Mirzade




## Citation
If you use HMNexus in academic research, please cite:

Salimy S., Asgari A., Shahbazi M., Ghasemi A., Mirzade M.
HMNexus: A Tkinter GUI Platform for High-Speed, Code-Free TCGA Data Download.
BMC Bioinformatics, 2025.

## License
© 2025 HMNexus Project
Released under the MIT License.


<div align="center">

🧬 HMNexus — Fast. Simple. Reliable TCGA Data Access.

</div> ```
