# glafit Bangladesh — Website Redesign Case Study

**Live site:** [codebyaminul.github.io/glafit-bangladesh](https://codebyaminul.github.io/glafit-bangladesh/) · **Repair portal:** [`/repair.html`](https://codebyaminul.github.io/glafit-bangladesh/repair.html)

The official website and self-service repair portal for **glafit Bangladesh Limited**, rebuilt from an outdated layout into a fast, motion-driven web experience.

---

## 1. Who is glafit Bangladesh?

glafit Bangladesh Limited is an urban green mobility company that brings compact Japanese electric mobility technology to Bangladesh. glafit started in Wakayama, Japan, and is backed by **Musashi Seimitsu Industry**, a Tier-1 Honda supplier. In Dhaka, glafit runs an integrated EV ecosystem for the gig economy and delivery logistics:

| Pillar | What it is |
| --- | --- |
| **Commercial fleet — `glafit SS`** | Heavy-duty, high-torque electric commercial bike powered by the Honda-engineered **Musashi 2KW e-Axle**. It is built for Dhaka's roads and monsoon waterlogging (**IP67** waterproof). |
| **60-second battery swapping** | Automated smart-locker stations at **PRAN-RFL Best Buy** outlets. Riders swap batteries instantly instead of waiting at a charging socket. |
| **IoT telematics** | **Grameenphone ALO Connect** 4G M2M connectivity for real-time GPS tracking, remote anti-theft immobilization and live battery health monitoring. |
| **Rider economics** | Flexible commercial leases from **৳2,200/week** with unlimited battery swaps, about **45% lower** operating cost than a petrol motorbike. |

---

## 2. What we built

1. **Brand architecture and navigation**
   - Rebuilt the header with a larger, high-contrast glafit Bangladesh logo on the left and clean navigation links on the right.
   - Removed redundant "Pre-Order" calls to action for a calmer, editorial look.
2. **Kinetic typography and parallax motion**
   - Section 02 ("Japanese Craft / Dhaka Streets") sets **CRAFT** in deep ink black against architectural grey to strengthen the visual hierarchy.
   - Two rows of text scroll in opposite directions, tied to [Lenis](https://github.com/darkroomengineering/lenis) smooth scroll.
3. **Interactive fleet and hardware showcase**
   - A model switcher spotlights the glafit SS commercial bike, the Musashi 2KW powertrain and the dual automotive-grade **51.2V LFP** battery packs.
   - Clear partner credits: Musashi / Honda, PRAN-RFL and Grameenphone.
4. **Battery swap process and cost comparison**
   - Step-by-step view of the 60-second locker swap: **Get Bike → Locate via App → 60s Scan & Swap → Ride Nonstop**.
   - Side-by-side comparison: **৳8,500–৳10,000/month** in petrol vs. the **৳2,200/week** all-inclusive glafit lease.
5. **App store links and telematics dashboard**
   - Live smartphone telemetry preview (92% charge, 96 km range, nearest-station radar).
   - Official Google Play and Apple App Store badges linking to the live apps.
6. **Dhaka headquarters (Uttara)**
   - Features the experience and diagnostics center on Sonargaon Janapath Road, Sector 12, Uttara.
   - Square map, opening hours (Sunday–Thursday) and a one-tap **"Get Live Route from My Location"** GPS button.
7. **Self-service support portal ([`repair.html`](repair.html))**
   - Diagnostic decision tree (`Yes` / `No` fault branching).
   - Component inspector with left/right bike schematics and highlighted hotspots.
   - Six step-by-step repair guides: battery, brakes, display, wheels, lighting and drivetrain.
   - Full factory technical specification sheet.
8. **Deployment and portfolio assets**
   - Deployed on GitHub Pages, with `.nojekyll` so the static files are served as-is.
   - Produced a 60-second 1080p walkthrough video and 7 high-resolution portfolio stills (kept out of git; see `.gitignore`).

---

## 3. What we want to achieve

- **Market trust and legitimacy:** Make glafit BD the benchmark for premium Japanese engineering and safety in Bangladesh's fast-electrifying market.
- **Fleet and rider acquisition:** Speed up pilot onboarding for delivery couriers (Pathao, Foodpanda and Daraz riders) with transparent weekly pricing and no battery purchase cost.
- **Host partnerships:** Get retail business owners and property managers to sign up as battery swapping station hosts.
- **Portfolio and client proof:** Show this project as a live, end-to-end case study of UI/UX design, frontend engineering, motion design and brand storytelling.

---

## 🚀 Quick start (local run)

There is no build step and no dependencies. Just run the bundled Node.js server:

```bash
git clone https://github.com/codebyaminul/glafit-bangladesh.git
cd glafit-bangladesh
node server.js   # serves on :8080 with HTTP range support for MP4 streaming
```

- Landing page: <http://localhost:8080/>
- Repair and service guide: <http://localhost:8080/repair.html>

---

## 📁 Repository structure

```
├── index.html            # Main landing page (hero, craft parallax, fleet, swap loop, costs, app, HQ)
├── repair.html           # Self-service repair & warranty portal
├── server.js             # Lightweight Node.js static server with HTTP range streaming
├── logo.png              # glafit Bangladesh wordmark
├── images/               # Product frames, bike schematics, app QR code
├── videos/               # 1080p background footage for the hero
├── img/, live_*.html,    # Snapshot of the previous (pre-redesign) site, kept for reference
│   live_style.css
├── CHAT_HISTORY.md       # Development session archive and prompt log
├── .nojekyll             # Serve files as-is on GitHub Pages
└── README.md
```

---

## 🛠 Tech stack

Hand-written HTML, CSS and vanilla JavaScript · Lenis smooth scroll · HTML5 video · GitHub Pages hosting · Node.js for local preview.
