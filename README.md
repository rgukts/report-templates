# B.Tech Major Project Report – RGUKT Srikakulam  

[![Overleaf](https://img.shields.io/badge/Overleaf-Ready-brightgreen.svg)](https://www.overleaf.com) [![LaTeX](https://img.shields.io/badge/LaTeX-Compiled-blue.svg)](https://github.com/rgukts/report-templates/releases) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![GitHub stars](https://img.shields.io/github/stars/rgukts/report-templates?style=social)](https://github.com/rgukts/report-templates) [![GitHub forks](https://img.shields.io/github/forks/rgukts/report-templates?style=social)](https://github.com/rgukts/report-templates) [![GitHub issues](https://img.shields.io/github/issues/rgukts/report-templates)](https://github.com/rgukts/report-templates/issues) [![GitHub release](https://img.shields.io/github/v/release/rgukts/report-templates)](https://github.com/rgukts/report-templates/releases)

A complete, university-approved LaTeX template for **B.Tech Major Project Reports** at **Rajiv Gandhi University of Knowledge Technologies, Srikakulam**.

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

[PDF Download – Latest Version](project_report_template.pdf)

**Repository:** [https://github.com/rgukts/report-templates](https://github.com/rgukts/report-templates)

---

### Repository Contents

```
├── main.tex                          ← Complete source (edit only top section)
├── logos/
│   ├── logo_red.png                  ← University logo (title page)
│   ├── logo_gold.png                 ← Alternative logo
│   ├── logo.png                      ← Standard logo
│   └── background_logo.png           ← Watermark (certificate pages)
├── project_report_template.pdf       ← Ready-to-submit compiled PDF
├── project_report_template.zip       ← Overleaf-ready source zip
├── LICENSE                           ← MIT License
└── README.md                         ← This file
```

---

### Quick Start (Overleaf – 30 seconds)

1. Download → [project_report_template.zip](project_report_template.zip)
2. Go to [overleaf.com](https://www.overleaf.com) → New Project → Upload Project
3. Upload the zip → Done! Start editing instantly.

---

### How to Customize (Only 15 lines to change!)

Open `main.tex` and edit **only these lines at the top**:

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
```

That's it! Everything else auto-updates.

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
✅ **Easy Customization** – Change only the top section  
✅ **Multiple Logo Options** – Includes red, gold, and standard logos  
✅ **Overleaf Ready** – Works seamlessly on Overleaf  
✅ **Well Documented** – Clear comments throughout the code  

---

### Customization Tips

1. **Replace Logo**: Update `logos/logo_red.png` with your official RGUKT logo
2. **Update Abstract**: Replace `\lipsum[1-3]` in the `\abstract` command with your actual abstract
3. **Add Content**: Remove dummy `\lipsum` text and add your real chapters, figures, tables, and references
4. **Modify Chapters**: Edit the example chapters starting at line 321 to match your project structure

---

### File Structure Details

- **main.tex**: Complete LaTeX source file with all formatting and structure
- **logos/**: Contains all logo files used in the document
  - `logo_red.png`: Used on title page
  - `background_logo.png`: Used as watermark on certificate/declaration pages
  - `logo_gold.png` & `logo.png`: Alternative logo options
- **project_report_template.pdf**: Compiled PDF ready for submission
- **project_report_template.zip**: Complete source package for Overleaf upload

---

### Contributing

Contributions are welcome! Feel free to:
- Report issues
- Suggest improvements
- Submit pull requests

---

**Made with ❤️ for RGUKT-Srikakulam students**  

Feel free to ⭐ star and fork!

---

### Credits

Created and maintained by [@alpharibbin](https://github.com/alpharibbin)

---

### License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
