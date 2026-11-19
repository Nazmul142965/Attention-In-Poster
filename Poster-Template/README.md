# Academic Poster LaTeX Template (Skeleton)

This folder contains a blank, reusable skeleton template based on `tikzposter` for creating clean, high-impact academic and algorithm conference posters (A0 Landscape).

---

## 📁 Files Included
- **`main.tex`**: The skeleton LaTeX template with ready-to-use 3-column layout, placeholders for equations, step-by-step algorithm flow, diagram boxes, complexity analysis, benchmark tables, and references.

---

## 🚀 How to Use / Compile

### Option 1: On Overleaf (Easiest)
1. Create a **New Project** -> **Upload Project** (or copy `main.tex` into an Overleaf project).
2. Go to **Menu** (top-left) in Overleaf.
3. Change **Compiler** from `pdfLaTeX` to **`XeLaTeX`** (or `LuaLaTeX`). This is required because of `fontspec` and custom font rendering.
4. Click **Recompile**.

### Option 2: Local Compilation
Using terminal / command line:
```bash
xelatex main.tex
```

---

## 🎨 Customization Guide

1. **Title, Author & Affiliation**:
   Edit lines 25–27 in `main.tex`:
   ```latex
   \title{Your Project Title}
   \author{Your Name}
   \institute{Your Department / University}
   ```

2. **Themes & Colors**:
   Change `\usetheme{Board}` to any built-in `tikzposter` theme:
   - `Board` (used by default)
   - `Default`, `Rays`, `Basic`, `Simple`, `Envelope`, `Wave`, `Autumn`, `Desert`

3. **Inserting Images / Diagrams**:
   Replace the diagram placeholder in Block 4 with:
   ```latex
   \includegraphics[width=0.7\linewidth]{your_image_file.png}
   ```

4. **Multi-language Support (e.g., Bengali)**:
   Uncomment:
   ```latex
   \newfontfamily\bangla{FreeSerif}[Script=Bengali]
   ```
   and wrap Bengali text in `{\bangla বাংলা লেখা}`.
