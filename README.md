# glafit Bangladesh — Official Website & Self-Service Repair Portal

Modern, cinematic editorial web platform for **glafit Bangladesh Limited**, showcasing intelligent Japanese hybrid electric mobility, 60-second battery swapping network, and factory-authorized self-service repair guides.

---

## ⚡ Overview & Architecture

- **Monochromatic B&W Editorial Styling**: High-contrast, minimalist `#000000` / `#0c0c0e` / `#ffffff` theme with custom glassmorphism surfaces and micro-interactions.
- **Cinematic 1080p Video Header**: Auto-cycling background commercial footage of the glafit SS electric bike with zero-latency HTML5 video playback.
- **Lenis Smooth Scroll**: Frictionless momentum scrolling and spring transitions.
- **Self-Service Repair Portal (`repair.html`)**:
  - Interactive Smart AI Diagnostic Decision Tree (`Yes` / `No` fault branching).
  - Component Inspector with left/right interactive bike schematics and glowing hotspot markers.
  - 6 Factory Step-by-Step Resolution Guides (Battery, Brakes, Display, Wheels, Lighting, Drivetrain).
  - Complete Factory Technical Specification Reference Sheet.
- **Session Transcript (`CHAT_HISTORY.md`)**: Full conversation history, design iterations, and prompt log.

---

## 🚀 Quick Start (Local Run)

No build step or complex dependencies required. Native Node.js HTTP server:

```bash
# Clone the repository
git clone https://github.com/codebyaminul/glafit-bangladesh.git
cd glafit-bangladesh

# Start local preview server (supports range requests for 1080p video streaming)
node server.js
```

Open your browser at:
- **Main Landing Page**: [http://localhost:8080/](http://localhost:8080/)
- **Repair & Service Guide**: [http://localhost:8080/repair.html](http://localhost:8080/repair.html)

---

## 📁 Repository Structure

```
├── index.html          # Main landing page (12 ordered sections, hero, specs, stations)
├── repair.html         # Dedicated repair portal (smart troubleshooter, hotspots, 6 guides)
├── server.js           # Lightweight Node.js server with HTTP range streaming for MP4s
├── logo.png            # Official glafit Bangladesh wordmark
├── images/             # Extracted 1080p product frames & bike schematic illustrations
│   ├── bike-left.png
│   ├── bike-right.png
│   ├── glafit-cockpit.jpg
│   ├── glafit-powertrain.jpg
│   └── glafit-rider.jpg
├── videos/             # 1080p commercial videos (upscaled & cropped)
│   ├── rider-forward.mp4
│   ├── scene-setup.mp4
│   └── studio-shot.mp4
├── CHAT_HISTORY.md     # Full development session archive & prompts
└── README.md
```

---

## 🇯🇵 About glafit
Founded in Wakayama, Japan in 2017 by CEO Teizo Narumi. In Bangladesh, glafit deploys Honda-backed Musashi e-Axle powertrains, PRAN-RFL Best Buy swapping locker infrastructure, and Grameenphone ALO Connect IoT telematics.
