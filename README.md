<div align="center">

<!-- ░░ NEON HEADER BANNER ░░ -->

```
╔══════════════════════════════════════════════════════════════╗
║     ██████╗ ███████╗███████╗██╗   ██╗███╗   ███╗███████╗     ║
║     ██╔══██╗██╔════╝██╔════╝██║   ██║████╗ ████║██╔════╝     ║
║     ██████╔╝█████╗  ███████╗██║   ██║██╔████╔██║█████╗       ║
║     ██╔══██╗██╔══╝  ╚════██║██║   ██║██║╚██╔╝██║██╔══╝       ║
║     ██║  ██║███████╗███████║╚██████╔╝██║ ╚═╝ ██║███████╗     ║
║     ╚═╝  ╚═╝╚══════╝╚══════╝ ╚═════╝ ╚═╝     ╚═╝╚══════╝     ║
╚══════════════════════════════════════════════════════════════╝
```

# ⚡ Software Engineer Resume Template

**A battle-tested, minimalist, ATS-optimized LaTeX resume template**  
*Purpose-built for Software Engineers · Mobile Developers · Tech Juniors*

---

[![License: MIT](https://img.shields.io/badge/License-MIT-cyan?style=for-the-badge&logo=opensourceinitiative&logoColor=black)](https://opensource.org/licenses/MIT)
[![Language: LaTeX](https://img.shields.io/badge/Language-LaTeX-blueviolet?style=for-the-badge&logo=latex&logoColor=white)](https://www.latex-project.org/)
[![ATS Friendly](https://img.shields.io/badge/ATS-Friendly%20✓-00ffcc?style=for-the-badge&logo=checkmarx&logoColor=black)](https://github.com/dev-amr-elsherif/software-engineer-resume-template)
[![One Page](https://img.shields.io/badge/Layout-One--Page-ff79c6?style=for-the-badge&logo=readthedocs&logoColor=black)](https://github.com/dev-amr-elsherif/software-engineer-resume-template)

</div>

---

## 🧠 Why This Template Exists

> The average recruiter spends **6 seconds** scanning a resume. Most templates fail tech juniors before they even get a callback.

This template was engineered to **eliminate that problem** — zero fluff, maximum signal. It is the product of deep research into how modern Applicant Tracking Systems parse LaTeX-generated PDFs and how senior technical recruiters evaluate early-career candidates.

| Challenge | This Template's Solution |
|:---|:---|
| 📄 Resume too long | Strict one-page layout with calibrated margins |
| 🤖 ATS fails to parse it | `pdfgentounicode=1` + `hidelinks` hyperref config |
| 🔍 Low keyword density | Section order optimized for technical keyword prominence |
| 🎨 Overdesigned layouts | Clean typographic hierarchy — no tables, no columns, no icons |
| 🧩 Hard to customize | Modular macro system — swap content without touching structure |

---

## 👁️ Live Preview & Instant Cloud Editing

No local setup required. Open the template directly on **Overleaf** and start editing in seconds:

<div align="center">

[![Open in Overleaf](https://img.shields.io/badge/Open%20in%20Overleaf-View%20%26%20Edit%20Live-47A141?style=for-the-badge&logo=overleaf&logoColor=white)](https://www.overleaf.com/read/wxvvcdjzxnng#d23995)

</div>

> **Tip:** Click the badge above → Overleaf opens with a **read-only view**. Hit **"Copy Project"** in the top menu to clone it to your own account and start editing immediately — no sign-in required to preview.

---

## ✨ Key Features

### `[01]` — One-Page Layout Optimization
Every spacing decision — margins, `\vspace`, `\resumeItemListEnd` padding — is mathematically tuned to maximize content density without sacrificing whitespace clarity. You get the most real estate possible on a single page.

### `[02]` — Flawless ATS Parsing
- `\pdfgentounicode=1` ensures the PDF is machine-readable at the glyph level
- `[hidelinks]` hyperref flag prevents link-box artifacts that confuse parsers
- Standard section titles (`Experience`, `Education`, `Skills`) recognized by all major ATS engines (Greenhouse, Lever, Workday)
- No multi-column layouts — single-column flow that parsers can read top-to-bottom

### `[03]` — Clean & Non-Cluttered Code Architecture
- Reusable macro commands: `\resumeItem`, `\resumeSubheading`, `\resumeProjectHeading`
- Separation of concerns: preamble (config) → macros (commands) → document (content)
- Zero redundant packages — every import has a purpose
- Annotated section markers for instant navigation

### `[04]` — Easy Customization
Swap your content in clearly labeled blocks — no LaTeX expertise required:

```
%-----------HEADING-----------     ← Your name, title, contacts
%-----------SUMMARY-----------     ← Professional summary (optional)
%-----------TECHNICAL SKILLS---    ← Skills table
%-----------PROJECTS-----------    ← Project entries
%-----------WORK EXPERIENCE----    ← Experience entries
%-----------EDUCATION----------    ← Degree(s)
%-----------CERTIFICATIONS-----    ← Certs & courses
%-----------LEADERSHIP---------    ← Volunteering / leadership
%-----------SOFT SKILLS--------    ← Soft skills & languages
```

---

## 🚀 Setup & Compilation Guide

### ☁️ Option A — Cloud (Zero Configuration) · *Recommended*

The fastest way to get started. No installation, no compiler setup.

1. Click → [![Open in Overleaf](https://img.shields.io/badge/Overleaf-Open%20Template-47A141?style=flat-square&logo=overleaf)](https://www.overleaf.com/read/wxvvcdjzxnng#d23995)
2. In the top menu, select **Menu → Copy Project**
3. Edit `resume.tex` directly in the browser
4. Hit **Recompile** — your PDF updates live ✓

> Overleaf handles all LaTeX dependencies automatically. No `MiKTeX`, no Perl, no extensions needed.

---

### 🖥️ Option B — Local Setup (VS Code + LaTeX Workshop)

For offline editing and full IDE features (IntelliSense, SyncTeX, PDF preview).

#### Prerequisites

| Tool | Purpose | Download |
|:---|:---|:---|
| **VS Code** | Editor / IDE | [code.visualstudio.com](https://code.visualstudio.com/) |
| **LaTeX Workshop** | VS Code extension for LaTeX | [VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop) |
| **MiKTeX** | LaTeX distribution (compiler + packages) | [miktex.org](https://miktex.org/download) |
| **Strawberry Perl** | Required by `latexmk` build tool | [strawberryperl.com](https://strawberryperl.com/) |

#### Step-by-Step

**1. Clone the repository**

```bash
git clone https://github.com/dev-amr-elsherif/software-engineer-resume-template.git
cd software-engineer-resume-template
```

**2. Install MiKTeX**

```
# Run the MiKTeX installer from https://miktex.org/download
# During setup: choose "Install missing packages on-the-fly" → Always
```

**3. Install Strawberry Perl**

```
# Download and run the installer from https://strawberryperl.com/
# Verify installation:
perl --version
```

**4. Install the LaTeX Workshop extension in VS Code**

```
ext install James-Yu.latex-workshop
```

**5. Open the project and compile**

```bash
# Open in VS Code
code .

# LaTeX Workshop will auto-detect resume.tex
# Press Ctrl+Alt+B  →  Builds the PDF
# Press Ctrl+Alt+V  →  Opens PDF preview side-by-side
```

> **Note:** On first build, MiKTeX will auto-download any missing packages. Ensure you have an internet connection for the initial compile.

#### Recommended VS Code Settings (`.vscode/settings.json`)

```jsonc
{
  "latex-workshop.latex.tools": [
    {
      "name": "latexmk",
      "command": "latexmk",
      "args": ["-pdf", "-synctex=1", "-interaction=nonstopmode", "%DOC%"]
    }
  ],
  "latex-workshop.view.pdf.viewer": "tab",
  "latex-workshop.latex.autoBuild.run": "onSave"
}
```

---

## 📁 Project Structure

```
software-engineer-resume-template/
│
├── resume.tex          ← Main LaTeX source (edit this)
├── resume.pdf          ← Compiled output (auto-generated)
├── .gitignore          ← Ignores LaTeX aux files
└── README.md           ← You are here
```

---

## 📜 License & Credits

This template is released under the **MIT License** — free to use, modify, and distribute, including for commercial purposes.

```
MIT License © 2025 Amr Fathy Elsherif
```

### Attribution

> This template is **heavily customized and optimized** by **Amr Fathy Elsherif**, built upon the original open-source base template by [**sb2nov**](https://github.com/sb2nov/resume) (MIT License).  
> Significant modifications include: ATS unicode configuration, custom macro architecture, section reordering for keyword prominence, and typography/spacing calibration.

---

## 👤 Author

<div align="center">

**Amr Fathy Elsherif**  
*Mobile Software Engineer · Electronics & Communications Engineering Student*

[![GitHub](https://img.shields.io/badge/GitHub-dev--amr--elsherif-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/dev-amr-elsherif)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-dev--amr--elsherif-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/dev-amr-elsherif/)

</div>

---

<div align="center">

*If this template helped you land an interview — drop a ⭐ on the repo. It means a lot.*

</div>
