# SKILOFRENIKHZ | 140+ BPM

Portfolio website and interactive beat machine for **SkiloFrenikhz** (Giovanni Ramos Garcia) — DJ and music producer from Piraju, SP, Brasil. Specializes in Psy Techno, Bounce and Acid Rave at 140+ BPM.

---

## Pages

| File | Description |
|------|-------------|
| `index.html` | Main portfolio — bio, tracks player, gig history, gallery, tech rider, booking |
| `skilo-beat-machine.html` | Interactive 16-step drum sequencer — Skilo Beat Machine v2.0 |

---

## Tech Stack

- **HTML5** — single-file pages, no build step required
- **Tailwind CSS** (CDN) — utility-first styling
- **Google Fonts** — Space Mono + Teko
- **Swiper.js** (CDN) — gallery carousel
- **Web Audio API** — synthesized drum sequencer (no sample files)

---

## Project Structure

```
skilofrenikhz/
├── index.html                     # Main portfolio page
├── skilo-beat-machine.html        # Interactive beat machine
├── assets/
│   ├── img/
│   │   ├── logo.png               # Brand logo
│   │   ├── persona.png            # DJ mascot illustration
│   │   ├── profile/
│   │   │   ├── foto-gi.png        # Artist press photo
│   │   │   └── foto-gi-tocando.png # Live performance photo
│   │   └── gallery/
│   │       ├── unistellar-3640.jpg
│   │       ├── unistellar-3674.jpg
│   │       ├── unistellar-3687.jpg
│   │       ├── unistellar-3693.jpg
│   │       └── unistellar-3749.jpg
│   └── audio/
│       ├── faixa-01.wav
│       ├── faixa-02.wav
│       ├── faixa-03.wav
│       └── faixa-04.wav
└── README.md
```

---

## Running Locally

No build step required. Open with any web server:

**XAMPP:**
```
Place project in: C:\xampp\htdocs\skilo\
Open: http://localhost/skilo/
```

**VS Code Live Server:**
```
Right-click index.html → Open with Live Server
```

**Python:**
```bash
python -m http.server 8080
# then open http://localhost:8080
```

---

## Features

- Brutalist design system with glitch effects and scan-line overlay
- Custom 🌰 cursor on mascot hover
- Interactive 3D tilt mascot card
- Swiper.js gallery carousel with 7 slides
- HTML5 Audio player with real tracks (faixa-01–04.wav)
- Scroll reveal animations
- WhatsApp booking form builder
- Full booking/press kit section
- **Skilo Beat Machine** — 6-channel, 16-step drum sequencer:
  - PSY KICK · ACID CLAP · CLOSED HAT · OPEN HAT · PSY BASS · TEKK STAB
  - BPM 120–160 (default 140) with swing
  - 4 pattern banks (A/B/C/D)
  - Tap Tempo, Mute/Solo per channel
  - Lowpass filter + Dub Delay FX
  - Frequency visualizer canvas

---

## Credits

**DJ / Artist:** Giovanni Ramos Garcia — SkiloFrenikhz  
**Booking:** Somma Agency  
**Development:** Claudio Santana — [Fluency Works](https://fluencyworks.com.br)

---

© 2026 SKILOFRENIKHZ | 140+ BPM · Todos os direitos reservados.
