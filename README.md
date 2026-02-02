# 🔱 Unified Chronology: One Year War — Universal Century GUNDAM

An interactive, scroll-driven timeline documenting the **canonical animated chronology** of Mobile Suit Gundam's Universal Century era, spanning **UC 0068 through UC 0097**.

[![Demo](https://img.shields.io/badge/Demo-Live%20Preview-blue?style=for-the-badge)](./demo.html)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](./LICENSE)

![Timeline Preview](https://img.shields.io/badge/Events-66-orange?style=flat-square)
![Series](https://img.shields.io/badge/Series-11-purple?style=flat-square)
![Years](https://img.shields.io/badge/Years%20Span-29-blue?style=flat-square)

---

## 🎯 Overview

This project cross-references every **TV series, OVA, and theatrical film** from Sunrise's Universal Century Gundam productions to construct a unified, day-level chronological timeline of canonical events. 

The timeline focuses on **animated productions only** as the authoritative canon source, following Sunrise's official position that "whatever's in the footage is official."

### Covered Productions

| Series | Year | UC Period |
|--------|------|-----------|
| Mobile Suit Gundam | 1979 | UC 0079 |
| Zeta Gundam | 1985-1986 | UC 0087-0088 |
| ZZ Gundam | 1986-1987 | UC 0088-0089 |
| Char's Counterattack | 1988 | UC 0093 |
| 0080: War in the Pocket | 1989 | UC 0079 |
| 0083: Stardust Memory | 1991-1992 | UC 0083 |
| 08th MS Team | 1996-1999 | UC 0079 |
| MS IGLOO | 2004-2009 | UC 0079 |
| Unicorn | 2010-2014 | UC 0096 |
| The Origin | 2015-2018 | UC 0068-0079 |
| Narrative | 2018 | UC 0097 |

---

## ✨ Features

### Interactive Timeline
- **66 canonical events** with detailed descriptions
- **Expandable event cards** — click to reveal full details, episode references, and faction information
- **Scroll-driven navigation** through five distinct eras

### Series Filtering
- Filter events by any combination of source series
- Instantly see how different productions overlap chronologically
- Compare event coverage across MSG, 08th MS Team, 0080, and more

### Colorblind-Safe Design
- **IBM Design / Wong palette** for universal accessibility
- Blue (Federation), Orange (Zeon), Pink (Multi-faction) color coding
- High contrast dark mode interface

### Event Classification
- **◆ Critical Events** — War-changing moments (Battle of A Baoa Qu, Axis Shock)
- **◇ Major Events** — Significant developments (Garma's death, Operation Rubicon)
- **○ Minor Events** — Supporting chronology (base captures, testing operations)

---

## 🚀 Quick Start

### Live Demo

Open `demo.html` in your browser for an instant preview:

```
/UC-GUNDAM/demo.html
```

The demo is a **standalone HTML file** with inline React/JSX — no build step required.

### Using the Component

The timeline is available as a React component:

```jsx
import GundamTimeline from './gundam-timeline.jsx';

function App() {
  return <GundamTimeline />;
}
```

#### Dependencies
- React 18+
- No additional dependencies required

---

## 📁 Project Structure

```
UC-GUNDAM/
├── demo.html              # Standalone demo (open in browser)
├── gundam-timeline.jsx    # React component
├── README.md              # This file
└── docs/
    └── timeline-research.md   # Source research document
```

---

## 🎨 Customization

### Adding Events

Events follow this schema:

```javascript
{
  id: 67,                           // Unique identifier
  date: "January 3, UC 0079",       // Display date
  dateSort: 79.0103,                // Sortable date (year.MMDD)
  title: "Event Title",             // Short title
  description: "Full description...", // Detailed text
  source: ["MSG", "MS IGLOO"],      // Source series (array)
  faction: "zeon",                  // federation | zeon | both | neutral
  significance: "critical",         // critical | major | minor
  episode: "Episode reference"      // Optional episode/movie reference
}
```

### Modifying Eras

Era groupings can be adjusted in the `eras` array:

```javascript
const eras = [
  { start: 68, end: 78, name: "PREQUEL ERA", subtitle: "Rise of Zeon" },
  { start: 79, end: 79.5, name: "ONE YEAR WAR", subtitle: "UC 0079" },
  // Add or modify eras here
];
```

---

## 📖 Canon Notes

### What's Included
- All Sunrise-produced animated Universal Century works from UC 0068-0097
- Events with documented in-universe dates (day-level where available)
- Cross-references showing how parallel productions depict the same time periods

### What's Excluded
- **Thunderbolt** — Officially designated "Another UC" parallel timeline
- **The Origin manga** — OVAs are included; manga contradicts original series
- **Games, novels, manga** — Not considered primary canon per Sunrise policy
- **MSV/design variations** — Model kit backstories not from animated works

### Known Discrepancies
When animated sources conflict, we follow these precedents:
- MS IGLOO dates for Battle of Loum (January 15-17) over Origin's January 23
- Original MSG deployment timelines over 08th MS Team's earlier GM appearances
- Later productions generally take precedence for expanded lore

---

## 🤝 Contributing

Contributions welcome! Please ensure any additions:
1. Come from **animated Sunrise productions only**
2. Include specific in-universe dates where documented
3. Note the source episode/film for verification

---

## 📜 License

MIT License — see [LICENSE](./LICENSE) for details.

**Gundam franchise** is © Sunrise Inc. / Sotsu Agency. This is a fan research project with no commercial affiliation.

---

## 📚 Citation

### Academic Citation

If you use this codebase in your research or project, please cite:

```bibtex
@software{uc_gundam_timeline,
  title = {Unified Chronology: One Year War — Universal Century GUNDAM Timeline},
  author = {Drift Johnson},
  year = {2025},
  url = {https://github.com/MushroomFleet/Unifed-Chronology--One-Year-War-Universal-Century-GUNDAM},
  version = {1.0.0}
}
```

### Donate

[![Ko-Fi](https://cdn.ko-fi.com/cdn/kofi3.png?v=3)](https://ko-fi.com/driftjohnson)
