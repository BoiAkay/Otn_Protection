# OTN Protection Switching: Complete Visual Guide & Interactive Simulator

An interactive, step-by-step educational guide to **Optical Transport Network (OTN) Protection Switching**, covering ITU-T standards G.873.1, G.873.2, G.709, G.798, and G.808.1.

## 🌟 Overview

When optical fiber is cut or an optical transceiver degrades, OTN Protection Switching automatically restores traffic in **under 50 milliseconds** — fast enough that phone calls and video streams don't drop. This project provides an interactive visualization of how carrier-grade telecom networks achieve this 99.999% availability ("five nines").

## ✨ Features

### 📚 8 Comprehensive Modules

1. **Fundamentals** — Why networks need sub-50ms switching, Bridge vs Selector concepts, Working vs Protection traffic
2. **Linear Protection Schemes** — Interactive animated diagrams of 1+1, 1:1, and 1:N architectures
3. **SNC Monitoring Modes** — Inherent (SNC/I), Sublayer (SNC/S), and Non-Intrusive (SNC/N) monitoring
4. **APS/PCC Protocol** — Interactive 32-bit protocol calculator and G.709 ODUk overhead map
5. **Ring Protection (OSPRing)** — Wrapping vs Steering mechanisms, squelch tables
6. **Live Interactive Simulator** — Real-time fiber cut injection, protection switch visualization
7. **Standards Summary** — Key rules and ITU-T document cross-reference
8. **Complete Table 8-1 Reference** — All 15 standardized linear protection architectures

### 🎮 Interactive Elements

- **Live Signal Flow Diagrams** — Real-time animated packet flows showing Working, Protection, and APS traffic
- **Fault Injection Controls** — Cut fibers, inject signal degradation, trigger Lockout of Protection
- **APS Protocol Calculator** — Build and decode 32-bit APS messages with priority resolution
- **G.709 Overhead Map** — Hover-annotated 4×16 byte frame structure showing where APS lives
- **Architecture Switcher** — Compare 1+1 Unidirectional, 1+1 Bidirectional, 1:1, and 1:N side-by-side

### 🎨 Design Features

- **Dark/Light Mode Toggle** — Full WCAG AA compliant color themes
- **Responsive Layout** — Works on desktop, tablet, and mobile
- **Zero Dependencies** — Pure HTML5, CSS3, and vanilla JavaScript
- **Offline First** — No external network requests, runs entirely in browser
- **Print Friendly** — Clean layout for PDF export

## 🚀 Quick Start

Simply open `otn_protection_guide.html` in any modern web browser (Chrome, Firefox, Safari, Edge). No build step, no server, no installation required.

```bash
# Clone the repository
git clone https://github.com/yourusername/Otn_Protection.git
cd Otn_Protection

# Open in browser
open otn_protection_guide.html
# or
firefox otn_protection_guide.html
```

## 📖 Usage

### Navigation

- Use the **sticky header menu** to jump to any module
- Click **architecture tabs** in Module 2 to compare protection schemes
- Press **theme toggle** (top-right) to switch between dark and light modes

### Interactive Simulator (Module 6)

1. Click **"Cut Working Fiber"** to inject a Loss of Signal (LOS) fault
2. Watch the selector arm flip to Protection in real-time
3. Observe the **APS protocol message** propagate between nodes
4. Review the **step-by-step execution log** showing millisecond-level timing
5. Click **"Repair Fiber"** to trigger the Wait-to-Restore (WTR) timer

### APS Protocol Calculator (Module 4)

1. Select a **Request Type** (Signal Fail, Signal Degrade, Manual Switch, etc.)
2. Choose **Architecture** (1+1 Permanent Bridge vs 1:N Switched)
3. Set **Direction** (Unidirectional vs Bidirectional)
4. View the computed **32-bit hex frame** and decoded explanation

## 📚 Included Standards (PDF Reference Documents)

The repository includes official ITU-T Recommendations for deep-dive reference:

- **G.709** (2020-06) — Interfaces for the optical transport network
- **G.798** (2026-02) — Characteristics of optical transport network hierarchy equipment functional blocks
- **G.808.1** (2014-05) — Generic protection switching – Linear trail and subnetwork protection
- **G.808.2** (2019-08) — Generic protection switching – Shared mesh protection
- **G.872** (2024-03) — Architecture of optical transport networks
- **G.873.1** (2017-10) — Optical transport network linear protection
- **G.873.2** (2015-08) — ODUk shared ring protection
- **G.873.3** (2017-09) — Optical transport network shared mesh protection

## 🛠️ Technical Stack

- **HTML5** — Semantic structure, SVG graphics
- **CSS3** — Tailwind CSS via CDN, custom animations
- **JavaScript (ES6+)** — Vanilla JS, no frameworks
- **SVG** — Dynamic path manipulation for signal flow visualization

## 🎯 Target Audience

- **Telecom Engineers** — Hands-on equipment configuration, network planning
- **Students** — Computer networks, optical communications courses
- **Certification Prep** — CCNA Service Provider, JNCIA-SP, Nokia NRS II
- **Technical Writers** — Understanding OTN for documentation
- **Anyone curious** about how carrier-grade telecom networks work

## 🔧 Browser Compatibility

Tested and working on:
- ✅ Chrome/Edge 90+
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Mobile Safari (iOS 14+)
- ✅ Chrome Mobile (Android 10+)

## 📝 Key Concepts Covered

- **Bridge & Selector** — Head-end replication vs tail-end selection
- **1+1 vs 1:1 vs 1:N** — Permanent vs switched bridging, extra traffic, shared protection
- **Revertive vs Non-Revertive** — Wait-to-Restore timer vs Do Not Revert mode
- **SNC/I, SNC/S, SNC/N** — Monitoring at server layer, TCM sublayer, or path layer
- **APS Protocol** — 4-byte signaling (Request, Requested Signal, Bridged Signal)
- **Priority Table** — Lockout > Forced Switch > Signal Fail > Signal Degrade > Manual Switch
- **Wrapping vs Steering** — Ring protection tradeoffs for metro vs long-haul
- **Squelch Table** — Misconnection prevention during multi-failure scenarios

## 🤝 Contributing

This is an educational project. If you find errors in the ITU-T standard interpretations, animation timing, or want to suggest improvements:

1. Fork the repository
2. Create a feature branch (`git checkout -b fix/animation-timing`)
3. Commit your changes (`git commit -m 'Fix protection switch timing in 1:1 diagram'`)
4. Push to the branch (`git push origin fix/animation-timing`)
5. Open a Pull Request

## 📜 License

This project is provided for **educational purposes**. The ITU-T PDF documents included are copyright © ITU and redistributed here for reference under ITU's terms for standards access.

The interactive HTML guide (`otn_protection_guide.html`) is released under the **MIT License** — free to use, modify, and distribute with attribution.

## 🙏 Acknowledgments

- **ITU-T Study Group 15** — For maintaining the OTN standards framework
- **Tailwind CSS** — For the utility-first styling approach
- **Claude (Anthropic)** — For assisting in development and verification

## 📧 Contact

For questions, corrections, or collaboration:
- Open an issue on GitHub
- Reach out via the repository discussions

---

**Star ⭐ this repository if you find it useful for learning OTN protection switching!**
