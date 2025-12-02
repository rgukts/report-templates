# B.Tech Major Project Report – RGUKT Srikakulam  

[![Overleaf](https://img.shields.io/badge/Overleaf-Ready-brightgreen.svg)](https://www.overleaf.com) [![LaTeX](https://img.shields.io/badge/LaTeX-Compiled-blue.svg)](https://github.com/rgukts/report-templates/releases) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![GitHub stars](https://img.shields.io/github/stars/rgukts/report-templates?style=social)](https://github.com/rgukts/report-templates)

A complete, university-approved LaTeX template for **B.Tech Major Project Reports** at **Rajiv Gandhi University of Knowledge Technologies, Srikakulam**.

---

## 📋 Table of Contents

- [Features](#features)
- [Cover Page Templates](#cover-page-templates)
- [Quick Start](#quick-start-overleaf--30-seconds)
- [Customization](#how-to-customize-only-15-lines-to-change)
- [Local Compilation](#local-compilation-optional)
- [Contributing](#contributing)
- [Credits](#credits)
- [License](#license)

---

Fully formatted as per RGUKT guidelines:

- Official title page with logo
- Certificate (Guide + HoD signature space)
- Declaration & Acknowledgement
- Abstract, TOC, LOF, LOT
- Double-line page border
- Proper Roman + Arabic pagination
- Professional sans-serif look (Source Sans Pro)

---

### Preview

📄 [PDF Download – Latest Version](project_report_template.pdf)

🔗 **Repository:** [github.com/rgukts/report-templates](https://github.com/rgukts/report-templates)

---

### Repository Contents

```
├── main.tex                          ← Complete source (edit only top section)
├── content.tex                       ← Customizable variables (project info)
├── logos/
│   ├── logo_red.png                  ← University logo (title page)
│   ├── logo_gold.png                 ← Gold logo (cover pages)
│   ├── logo_black.png                ← Black logo (cover pages)
│   ├── logo.png                      ← Standard logo
│   └── background_logo.png           ← Watermark (certificate pages)
├── cover page/                       ← Alternative cover page templates
│   ├── gold text light background/
│   │   └── name.tex                  ← Gold text on light background template
│   ├── gold text dark background/
│   │   └── name.tex                  ← Gold text on dark background template
│   ├── dark text light background/
│   │   └── name.tex                  ← Dark text on light background template
│   └── borders/                      ← Decorative border images for cover pages
│       ├── gold_border.png           ← Gold border (for gold text templates)
│       ├── gold_border_dark.png      ← Gold border dark variant
│       └── black_border.png          ← Black border (for dark text template)
├── project_report_template.pdf       ← Ready-to-submit compiled PDF
├── project_report_template.zip       ← Overleaf-ready source zip
├── LICENSE                           ← MIT License
└── README.md                         ← This file
```

---

### Cover Page Templates

This repository includes **multiple cover page options** to suit different preferences:

1. **Gold Text Light Background** (`cover page/gold text light background/name.tex`)
   - Elegant gold text (RGB: 212,175,55) on light background
   - Uses `logo_gold.png` and `borders/gold_border.png`
   - Perfect for formal submissions
   - Border: Gold decorative border image

2. **Gold Text Dark Background** (`cover page/gold text dark background/name.tex`)
   - Gold text on dark background
   - Uses `logo_gold.png` and `borders/gold_border_dark.png`
   - Professional dark theme
   - Border: Gold border with dark background variant

3. **Dark Text Light Background** (`cover page/dark text light background/name.tex`)
   - Classic black text on light background
   - Uses `logo_black.png` and `borders/black_border.png`
   - Traditional academic style
   - Border: Black decorative border image

4. **Standard Template** (in `main.tex`)
   - Default template with double-line border (TikZ drawn)
   - Uses `logo_red.png`
   - Standard RGUKT format
   - Border: Programmatically drawn double-line border

**Template Structure:**
- Each template folder contains `name.tex` - the standalone LaTeX file for that cover page style
- All templates `\input{content}` to use variables from `content.tex`
- Border images are stored in `cover page/borders/` folder
- Each template uses appropriate logo and border combination

**To use an alternative cover page:**
- Copy the desired `name.tex` file from `cover page/` folder
- Replace the title page section in `main.tex` with the chosen template
- Ensure border images are accessible (they're referenced relative to the template location)
- All templates use the same variables from `content.tex` for easy customization

---

### Quick Start (Overleaf – 30 seconds)

1. **Download** → [project_report_template.zip](project_report_template.zip)
2. **Go to** [overleaf.com](https://www.overleaf.com) → **New Project** → **Upload Project**
3. **Upload** the zip file → Done! Start editing instantly.

> 💡 **Tip:** The template is pre-configured and ready to use. Just customize the top section of `main.tex` with your project details.

---

### How to Customize (Only 15 lines to change!)

Open `content.tex` and edit **only these lines**:

```latex
\newcommand{\projectname}{Your Actual Project Title}
\newcommand{\guidename}{Mr./Dr. Guide Name}
\newcommand{\guidequal}{M.Tech , Ph.D}
\newcommand{\qualification}{Assistant professor}
\newcommand{\hodname}{Mr./Dr. HOD Name}
\newcommand{\hodqual}{Assistant professor}

\newcommand{\studentone}{Student Name 1}
\newcommand{\studenttwo}{Student Name 2}
\newcommand{\studentthree}{Student Name 3}
\newcommand{\studentfour}{Student Name 4}
\newcommand{\studentfive}{Student Name 5}
\newcommand{\studentsix}{Student Name 6}
% Add/remove as needed (up to 6 supported)

\newcommand{\studentidone}{S200XXX}
\newcommand{\studentidtwo}{S20XXXX}
% ... continue for all students

\newcommand{\branch}{Electronics and Communication Engineering}
\newcommand{\campus}{Rajiv Gandhi University of Knowledge Technologies - Srikakulam}
\newcommand{\submissiondate}{November - 2025}  % Customize submission date
```

That's it! Everything else auto-updates. All cover page templates will use these same variables.

---

### Local Compilation (Optional)

```bash
pdflatex main.tex
pdflatex main.tex    # Run twice for TOC & page numbers
# or
latexmk -pdf main.tex
```

**Requirements:**
- LaTeX distribution (TeX Live, MiKTeX, or MacTeX)
- All packages listed in the preamble (automatically installed by most distributions)

---

### Features

✅ **Complete Structure** – All required pages included  
✅ **Professional Formatting** – Double-line border, proper spacing, modern fonts  
✅ **Multiple Cover Page Options** – 4 different cover page templates to choose from  
✅ **Easy Customization** – Change only the variables in `content.tex`  
✅ **Multiple Logo Options** – Includes red, gold, black, and standard logos  
✅ **Overleaf Ready** – Works seamlessly on Overleaf  
✅ **Well Documented** – Clear comments throughout the code  

---

### Customization Tips

1. **Choose Cover Page**: Select from 4 different cover page templates (standard, gold light, gold dark, or dark text)
2. **Replace Logo**: Update logo files in `logos/` folder with your official RGUKT logos
3. **Set Submission Date**: Update `\submissiondate` in `content.tex` (e.g., "May - 2024" or "November - 2025")
4. **Update Abstract**: Replace `\lipsum[1-3]` in the `\abstract` command in `content.tex` with your actual abstract
5. **Add Content**: Remove dummy `\lipsum` text and add your real chapters, figures, tables, and references
6. **Modify Chapters**: Edit the example chapters in `main.tex` to match your project structure

---

### File Structure Details

- **main.tex**: Complete LaTeX source file with all formatting and structure (standard template)
- **content.tex**: All customizable variables (project name, students, guide, etc.)
- **logos/**: Contains all logo files used in the document
  - `logo_red.png`: Used on standard title page
  - `logo_gold.png`: Used in gold-themed cover pages
  - `logo_black.png`: Used in dark text cover pages
  - `background_logo.png`: Used as watermark on certificate/declaration pages
- **cover page/**: Alternative cover page templates
  - **gold text light background/name.tex**: Standalone template with gold text on light background, uses `gold_border.png`
  - **gold text dark background/name.tex**: Standalone template with gold text on dark background, uses `gold_border_dark.png`
  - **dark text light background/name.tex**: Standalone template with black text on light background, uses `black_border.png`
  - **borders/**: Decorative border image files
    - `gold_border.png`: Gold decorative border for light background templates
    - `gold_border_dark.png`: Gold decorative border for dark background templates
    - `black_border.png`: Black decorative border for dark text templates
- **project_report_template.pdf**: Compiled PDF ready for submission
- **project_report_template.zip**: Complete source package for Overleaf upload

---

### Contributing

Contributions are welcome! Feel free to:
- 🐛 [Report issues](https://github.com/rgukts/report-templates/issues)
- 💡 Suggest improvements
- 🔀 Submit pull requests

Your contributions help make this template better for all RGUKT students!

---

**Made with ❤️ for RGUKT-Srikakulam students**  

⭐ **Star this repo** if you find it helpful!  
🔀 **Fork** to customize for your needs!

---

### Credits

Created and maintained by [@alpharibbin](https://github.com/alpharibbin)

---

### License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
