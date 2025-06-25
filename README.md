# Protocol Audit Report

![ZNTB Logo](./logo.pdf) <!-- or logo.png if you prefer -->

## 📝 Overview
This repository contains the security audit report for **<https://github.com/zntb/3-passwordstore-audit>**, conducted by [zntb](https://github.com/zntb).

## 📂 Contents
- `report.pdf` - Final audit report (PDF version)

## 🔍 Key Findings
| Severity | Count |
|----------|-------|
| High     | 2     |
| Medium   | 0     |
| Low      | 0     |
| Info     | 1     |

**Critical Findings:**
1. [H-1] Storing password on-chain makes it publicly visible
2. [H-2] Missing access control in `setPassword` function

## 🛠️ How to Generate the PDF
1. Install dependencies:
   ```bash
   sudo apt install pandoc texlive-latex-extra texlive-fonts-recommended
   ```
2. Generate from Markdown:
   ```bash
   pandoc report.md -o report.pdf \
  --template=eisvogel \
  --pdf-engine=xelatex \
  --listings
  ```
📄 Template Used
<https://github.com/Wandmalfarbe/pandoc-latex-template>

📅 Audit Period
June 2025
