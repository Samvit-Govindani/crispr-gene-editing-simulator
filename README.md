# crispr-gene-editing-simulator
Interactive, offline CRISPR-Cas9 simulator with clickable PAM sites, gRNA design, and step-by-step animation.
# CRISPR-Vis: Interactive Gene-Editing Simulator (Offline)

An **educational, browser-based CRISPR-Cas9 simulator** that lets you:
- Visualize a 3D DNA double helix and **click real PAM-like sites**.
- Automatically **design a 20-nt protospacer & guide (reverse-complement)**.
- See a **step-by-step animation** of gRNA design → Cas9 binding → cut → HDR repair.
- Switch **PAM patterns** (SpCas9 NGG, NGA variant, xCas9 NG) and **load custom DNA**.
- Export the designed **gRNA** (FASTA + JSON) and **download a snapshot** of the scene.

> ⚠️ **Disclaimer**  
> This is an educational visualization. It is **not** a validated design tool and **must not** be used for clinical decision-making. Provided *as is* under the MIT License.

---

## 🎯 Why this project
This simulator turns textbook CRISPR steps into something you can **see and explain**. It’s designed to show:
- Practical computational biology concepts (PAMs, guide design).
- Thoughtful engineering: **offline**, **no API keys**, **deterministic UI**, clear comments.
- Communication: info panel explanations and exportable artifacts.

---

## ✨ Features
- **3D DNA helix** (Three.js + OrbitControls) with clickable PAM sites (magenta).
- **PAM chooser:** NGG / NGA / NG (toy regex patterns).
- **gRNA design:** 20-nt protospacer (upstream of PAM) + reverse-complement **guide**.
- **Heuristics:** GC% and a simple, naive off-target warning (for teaching; not a genome search).
- **Animation:** gRNA design → Cas9 binding → double-strand break → HDR repair.
- **Custom sequences:** paste your own A/T/C/G DNA.
- **Exports:** gRNA as **FASTA** and **JSON**, **PNG snapshot** of the viewer.
- **Accessibility:** reduced-motion friendly; descriptive info panel.
- **Multiple disease options**

---

## 🛠 Tech Stack
- **Three.js r128** + **OrbitControls** (3D)
- **GSAP** (timeline animation)
- **Tailwind CSS** (UI)
- **Vanilla JS** (no build, no server)

---

## 🚀 Getting Started
1. Clone or download the repo.  
2. Open `index.html` in a modern browser (Chrome/Edge/Firefox/Safari).  
3. (Optional) Enable **GitHub Pages** → “Deploy from branch” → `main` → `/root`.  
   Your app will be live at: `https://<your-username>.github.io/<repo-name>/`

> Tip: Keep the filename as `index.html` so Pages serves it automatically.
