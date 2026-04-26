# CGOW — Godot Open World (Demo)

> An open-world multiplayer game built in Godot 4 — featuring vehicles, inventory, weapons, combat, NPCs, and an AI-generated mission system.

![Godot 4](https://img.shields.io/badge/Godot-4.x-478CBF?logo=godot-engine&logoColor=white)
![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20Android-green)
![Status](https://img.shields.io/badge/Status-Demo%20%2F%20WIP-orange)

---

## About

This is a **work-in-progress demo** project showcasing a range of production-ready Godot 4 systems working together in a single open-world environment. It is built by [Sanjay Meher](https://cggodotassets.shop) as a technical portfolio piece — all major systems used here are available as drop-in assets at the store.

---

## Features

| System | Description |
|---|---|
| 🚗 Multiplayer Vehicles | Drive and ride with other players across the open world |
| 🎒 Inventory System | Drag-and-drop item management and equipment |
| 🔫 Weapons & Combat | Ranged and melee combat system |
| 🤖 NPC & Enemy AI | Melee + ranged enemies with dynamic behavior |
| 🧠 AI Mission Generator | Groq/Gemini powered dynamic mission system |
| 🌍 Open World Map | Large explorable world with multiple zones |
| 📱 Mobile Support | Full Android support with mobile controls |

---

## Project Structure

```
CGOW/
├── scenes/          # All .tscn scene files
│   ├── Maps/        # World and level scenes (airport.tscn etc.)
│   ├── NPCai.tscn   # AI NPC scene
│   └── ...
├── scripts/         # GDScript logic
│   ├── BR/          # Battle Royale / job NPC scripts
│   ├── GameNPC.gd   # NPC controller
│   ├── MissionGenerator.gd  # AI mission logic
│   └── ...
├── assets/          # Textures, audio, models
└── README.md
```

---

## Setup for Collaborators

### Requirements
- [Godot 4.x](https://godotengine.org/download)
- Android export templates (for Android builds)

### Getting Started

```bash
# Clone the repo
git clone https://github.com/sanjaymeherdev/Godot-Open-World.git

# Open in Godot 4
# File → Open Project → select the project folder
```

### API Keys (Required)

This project uses AI APIs for the mission generator and NPC dialogue. You need to set your own keys.

1. Open `scripts/MissionGenerator.gd` — set your Groq API key on line 7
2. Open `scripts/GameNPC.gd` — set your Groq API key on line 16
3. Open `scripts/BR/jobNPC.gd` — set your Groq API key on line 10

> ⚠️ **Never commit API keys to the repo.** Add a `.gitignore` entry or use ProjectSettings for key storage.

Get a free Groq key at [console.groq.com](https://console.groq.com)

---

## Platforms

| Platform | Status |
|---|---|
| Windows | ✅ Supported |
| Android | ✅ Supported |
| Linux / Mac | ❓ Untested |

---

## Assets & Systems Used

All systems in this project are built and maintained by the developer and available at:

👉 **[cggodotassets.shop](https://cggodotassets.shop)**

Key systems from the store used here:
- CGRelay — Multiplayer relay server
- Inventory Drag & Drop
- Weapon System (Tres-based)
- Enemy AI — Melee + Ranged
- AI Integrations (Groq, Gemini)
- Mobile Controls + Gyro

---

## Known Issues (Demo)

- Some areas of the map are incomplete
- AI missions may occasionally produce repetitive results
- Mobile performance varies by device
- Multiplayer desync possible on high-latency connections

---

## Contact & Collaboration

- 🌐 Website: [cggodotassets.shop](https://cggodotassets.shop)
- 💬 WhatsApp: [Chat with Sanjay](https://wa.me/917504704502)
- 🛒 Store: [Browse 50+ Godot Systems](https://cggodotassets.shop/cgstore)

---

*Built with ❤️ in Godot 4 — Made in India 🇮🇳*
