# Harsh Mishra — Portfolio Website

> **Silicon to Intelligence** — Designing processors, digital systems and intelligent radar-based solutions.

[![Live Site](https://img.shields.io/badge/Live%20Site-enggoharsh.github.io-0ab4ff?style=flat-square&logo=github)](https://enggoharsh.github.io)
[![License](https://img.shields.io/badge/License-MIT-00e5ff?style=flat-square)](LICENSE)
[![HTML](https://img.shields.io/badge/Built%20With-HTML%20%2F%20CSS%20%2F%20JS-00d4aa?style=flat-square)](index.html)

---

## Overview

Personal portfolio website for **Harsh Mishra** — RTL Design Engineer, FPGA Developer, and RISC-V Processor Designer. Built as a single, zero-dependency HTML file with a dark futuristic aesthetic inspired by PCB traces, silicon dies, and processor datapaths.

No frameworks. No build step. No Node.js. Just open `index.html` and it works.

---

## Live Demo

```
https://enggoharsh.github.io
```

---

## Sections

| # | Section | What's Inside |
|---|---------|---------------|
| 01 | **Hero** | Animated particle grid, floating RISC-V instruction stream, name + title |
| 02 | **About** | Engineering timeline, key stats (37 instructions, 125 MHz, 88% accuracy, 8.36 CGPA) |
| 03 | **Skills** | RTL/Hardware, EDA Tools, Programming, AI/DSP skill cards |
| 04 | **Projects** | RV32I Processor, SAP-2 CPU, UART (live simulator), FMCW Radar HAR |
| 05 | **Experience** | NIT Patna Research Internship — animated terminal interface |
| 06 | **Achievements** | GATE ECE, NPTEL Elite+Silver, Vice Chancellor Awards, Research Intern |
| 07 | **Leadership** | VLSI Lead @ Tarang Club — team metrics + workshop curriculum |
| 08 | **Contact** | Formspree-powered form → delivers to Gmail, social links |

---

## Featured Projects

### 1. 32-bit RISC-V Processor (RV32I ISA) — Flagship
- Single-cycle architecture, 37 instructions (R/I/S/B/U/J-type)
- Deployed on PYNQ-Z2 FPGA @ **125 MHz**
- Resource utilization: LUTs 2415 (4.54%), FFs 1085 (1.02%), BRAM 4 (2.85%)
- Animated datapath visualization with live data-packet flow
- Tools: Verilog HDL, AMD Vivado

### 2. SAP-2 8-bit CPU
- Complete RTL datapath + control logic in synthesizable Verilog
- Fetch → Decode → Execute pipeline
- FPGA hardware validated on PYNQ-Z2
- Tools: Verilog HDL, Vivado

### 3. UART Serial Communication System
- FSM-based full UART (Tx/Rx + baud-rate generator)
- 9600 baud, 16× oversampling, parity checking, configurable stop-bit
- Includes **live in-browser UART frame visualizer** — type any character, see the frame animate bit-by-bit
- Tools: Verilog HDL, Vivado

### 4. FMCW Radar Human Activity Recognition — Research
- End-to-end pipeline: Raw Radar → CWT → Scalogram → CNN → Classification
- 1800 samples across 6 activity classes, 70/15/15 split
- Best accuracy: **88.28%** (GoogLeNet + SVM)
- Benchmarked 5 classification pipelines
- Tools: TensorFlow, Keras, OpenCV, NumPy

---

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Markup | HTML5, semantic structure |
| Styling | CSS3, CSS custom properties (variables), clamp(), clip-path |
| Animation | Canvas API (particle grid), SVG animateMotion, CSS keyframes |
| Fonts | JetBrains Mono, Syne, Space Grotesk (Google Fonts) |
| Contact Form | Formspree (free tier) |
| Hosting | GitHub Pages |
| Dependencies | **Zero** — no npm, no bundler, no framework |

---

## Getting Started

### Run Locally

```bash
# Clone the repo
git clone https://github.com/enggoharsh/enggoharsh.github.io.git

# Open directly in browser — no server needed
open index.html
# or on Windows:
start index.html
```

That's it. No `npm install`. No build command.

### Deploy to GitHub Pages

```bash
# 1. Create a repo named exactly:
#    enggoharsh.github.io

# 2. Push your file
git init
git add index.html README.md
git commit -m "feat: initial portfolio launch"
git branch -M main
git remote add origin https://github.com/enggoharsh/enggoharsh.github.io.git
git push -u origin main

# 3. Go to GitHub → Settings → Pages → Source: main branch
# 4. Live at https://enggoharsh.github.io in ~2 minutes
```

---

## Contact Form Setup (Formspree)

The contact form sends messages directly to your Gmail. One-time setup required:

**Step 1** — Register at [formspree.io](https://formspree.io/register) using `enggoharsh@gmail.com`

**Step 2** — Click **+ New Form** → name it "Portfolio Contact"

**Step 3** — Copy your form ID (looks like `xpwzqdkr`)

**Step 4** — Open `index.html`, find this line and replace `YOUR_FORM_ID`:

```html
action="https://formspree.io/f/YOUR_FORM_ID"
```

**Step 5** — Save, commit, push. Done — messages land in your Gmail inbox.

Free tier allows **50 submissions/month**, which is more than enough for a portfolio.

---

## Customization

All personal data is in the HTML — no config files, no CMS. To update:

| What to change | Where to find it |
|---------------|-----------------|
| Name / title / tagline | `#hero` section |
| Timeline events | `#about` → `.timeline` |
| Skill tags | `#skills` → `.skill-tags` |
| Project details & metrics | `#projects` section |
| Terminal experience lines | JS `lines` array near `termBody` |
| Achievement cards | `#achievements` section |
| Leadership numbers | `.leadership-metrics` |
| Contact links | `#contact` → `.contact-info` |
| Color scheme | `:root` CSS variables at top of `<style>` |

### Color Variables

```css
--black:        #020408   /* page background */
--blue:         #0ab4ff   /* primary accent */
--cyan:         #00e5ff   /* secondary accent */
--teal:         #00d4aa   /* success / highlights */
```

---

## Performance

- Single file, no external JS dependencies
- Google Fonts loaded with `rel="preconnect"` for speed
- Canvas animation runs at 60fps with minimal CPU usage
- No render-blocking resources
- Works offline after first load (fonts cached by browser)

---

## Project Structure

```
enggoharsh.github.io/
├── index.html      ← entire website (single file)
└── README.md       ← this file
```

---

## Contact

| Platform | Link |
|---------|------|
| Email | enggoharsh@gmail.com |
| GitHub | [github.com/enggoharsh](https://github.com/enggoharsh) |
| LinkedIn | [linkedin.com/in/harshrajeshmishra](https://linkedin.com/in/harshrajeshmishra) |
| Phone | +91 889-923-4364 |

---

## License

 Apache License: Version 2.0, January 2004


---

*Built with Verilog in the heart, HTML in the hands.*
