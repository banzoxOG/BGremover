<div align="center">

<br/>

```
  ██████╗ ██████╗ ██████╗ ███████╗███╗   ███╗ ██████╗ ██╗   ██╗███████╗██████╗ 
  ██╔══██╗██╔════╝ ██╔══██╗██╔════╝████╗ ████║██╔═══██╗██║   ██║██╔════╝██╔══██╗
  ██████╔╝██║  ███╗██████╔╝█████╗  ██╔████╔██║██║   ██║██║   ██║█████╗  ██████╔╝
  ██╔══██╗██║   ██║██╔══██╗██╔══╝  ██║╚██╔╝██║██║   ██║╚██╗ ██╔╝██╔══╝  ██╔══██╗
  ██████╔╝╚██████╔╝██║  ██║███████╗██║ ╚═╝ ██║╚██████╔╝ ╚████╔╝ ███████╗██║  ██║
  ╚═════╝  ╚═════╝ ╚═╝  ╚═╝╚══════╝╚═╝     ╚═╝ ╚═════╝   ╚═══╝  ╚══════╝╚═╝  ╚═╝
```

**Remove backgrounds from any photo — instantly, for free, in your browser.**

[![Live Demo](https://img.shields.io/badge/🌐_Live_Demo-banzoxog.github.io/BGremover-00d4ff?style=for-the-badge&labelColor=06060c)](http://banzoxog.github.io/BGremover)
![No Server](https://img.shields.io/badge/No_Server-100%25_Client_Side-8b5cf6?style=for-the-badge&labelColor=06060c)
![No Signup](https://img.shields.io/badge/No_Signup-Free_Forever-ec4899?style=for-the-badge&labelColor=06060c)
![MIT License](https://img.shields.io/badge/License-MIT-22d3ee?style=for-the-badge&labelColor=06060c)

<br/>

</div>

---

## ✦ What is BGremover?

**BGremover** is a sleek, browser-based background removal tool. Drop in a photo, drag a slider, and download a clean transparent PNG — all without uploading anything to a server, creating an account, or paying a dime.

Everything runs **100% on your device** using the browser's Canvas API.

---

## ✦ Features

| Feature | Details |
|---|---|
| 🖱️ **Drag & Drop** | Drop any image directly onto the page |
| ⚡ **Instant Processing** | No upload wait — processed locally in seconds |
| 🎛️ **Sensitivity Slider** | Fine-tune how aggressively the background is detected |
| 🌫️ **Edge Softness** | Smooth out edges for a natural, clean cutout |
| ↔️ **Before / After Slider** | Drag to compare original vs. result side by side |
| 💾 **Full Quality Download** | Downloads as transparent PNG at original resolution |
| 🔒 **100% Private** | Your images never leave your device |
| 📱 **Responsive** | Works on desktop and mobile |

---

## ✦ How to use

```
1. Go to http://banzoxog.github.io/BGremover
2. Drop your image or click to browse
3. Wait a moment for processing
4. Drag the comparison slider to preview
5. Adjust sensitivity / edge softness if needed → hit Reapply
6. Click Download PNG
```

> **Best results:** Works great on photos with solid or simple backgrounds (white, studio, flat color). Complex backgrounds like forests or crowds may need manual tweaking with the sensitivity slider.

---

## ✦ Tech stack

```
HTML5          → Structure
CSS3           → Animations, glassmorphism, grid layout
Vanilla JS     → Zero frameworks, zero dependencies
Canvas API     → Image processing & pixel manipulation
Google Fonts   → Syne + Figtree + DM Mono
```

No npm. No build step. No backend. Just one `index.html`.

---

## ✦ How it works

BGremover uses a **flood-fill algorithm** starting from the edges of the image:

```
1. Sample corner + edge pixels → determine background color
2. BFS flood-fill from all 4 edges inward
3. Any pixel within color-distance threshold → marked transparent
4. Gaussian blur pass on the alpha channel → soft edges
5. Export as PNG with full transparency
```

This approach works well for photos where the background connects to the image border (most studio shots, product photos, portraits).

---

## ✦ Run locally

No build process needed — just open the file:

```bash
git clone https://github.com/banzoxog/BGremover.git
cd BGremover
open index.html   # or just double-click it
```

---

## ✦ Deploy your own

```bash
# Fork this repo, then:
# Go to Settings → Pages → Source: main / root → Save
# Your site goes live at https://yourusername.github.io/BGremover
```

---

## ✦ Project structure

```
BGremover/
└── index.html      ← the entire app (HTML + CSS + JS, single file)
└── README.md       ← you are here
```

---

## ✦ License

MIT — do whatever you want with it.

---

<div align="center">

Made by **banzoxog** &nbsp;·&nbsp; [Live Site](http://banzoxog.github.io/BGremover) &nbsp;·&nbsp; Give it a ⭐ if you like it

</div>
