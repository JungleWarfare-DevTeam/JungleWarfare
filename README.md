<div align="center">

```
 ██╗██╗   ██╗███╗   ██╗ ██████╗ ██╗     ███████╗
 ██║██║   ██║████╗  ██║██╔════╝ ██║     ██╔════╝
 ██║██║   ██║██╔██╗ ██║██║  ███╗██║     █████╗  
 ██║██║   ██║██║╚██╗██║██║   ██║██║     ██╔══╝  
 ██║╚██████╔╝██║ ╚████║╚██████╔╝███████╗███████╗
 ╚═╝ ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝ ╚══════╝╚══════╝
          W A R F A I R
```

**A deep-jungle tactical combat game — built to be broken, rebuilt, and modded.**

[![Latest Release](https://img.shields.io/github/v/release/your-org/jungle-warfair?style=for-the-badge&color=4a7c59&label=Latest+Release)](../../releases/latest)
[![Downloads](https://img.shields.io/github/downloads/your-org/jungle-warfair/total?style=for-the-badge&color=2d5a27&label=Total+Downloads)](../../releases)
[![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)](LICENSE)
[![Mod Support](https://img.shields.io/badge/Mod_Support-✔_Full-brightgreen?style=for-the-badge)](#-modding)
[![Discord](https://img.shields.io/badge/Discord-Join_Community-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/your-invite)

</div>

---

## 📦 Downloads & Releases

> **This is the official public releases repository for Jungle Warfair.**  
> Stable builds, beta previews, and hotfixes are all published here.

| Channel | Description | Stability |
|---|---|---|
| 🟢 **Stable** | Fully tested, recommended for all players | ✅ Production-ready |
| 🟡 **Beta** | Feature-complete but may have rough edges | ⚠️ Mostly stable |
| 🔴 **Nightly** | Experimental bleeding-edge builds | ❌ Expect bugs |

### ⬇️ [Go to Releases →](../../releases)

Each release includes:
- Windows (`.exe` installer & portable `.zip`)
- Linux (`.AppImage` & `.tar.gz`)
- macOS (`.dmg`)
- Full mod SDK and example mods
- Changelog and patch notes

---

## 🎮 About the Game

**Jungle Warfair** is a tactical combat game set in dense, procedurally generated jungle environments. Command your squad through hostile terrain, manage resources, and outmaneuver enemies hidden beneath a canopy that hides as many dangers as your opponents do.

- 🌿 **Dynamic jungle environments** — terrain, weather, and wildlife all affect combat
- 🧠 **Tactical squad AI** — give orders and let your team execute
- 🔫 **Deep weapon & gear systems** — every loadout decision matters
- 🗺️ **Procedural map generation** — no two missions are the same
- 🛠️ **Built from the ground up for modding**

---

## 🛠️ Modding

Jungle Warfair was designed with modding as a first-class feature. Nearly every system in the game can be extended, replaced, or overhauled.

### What Can Be Modded

| System | Moddable | Notes |
|---|---|---|
| Maps & Terrain | ✅ | Custom biomes, tilesets, and generators |
| Weapons & Equipment | ✅ | Full stat control, custom models |
| Enemies & Factions | ✅ | New AI behaviors, unit types |
| Game Modes | ✅ | Script your own win conditions |
| UI & HUD | ✅ | Full layout and styling control |
| Sound & Music | ✅ | Drop-in audio replacement |
| Core Engine | ⚠️ | Limited — contact devs for deep hooks |

### Getting Started with Mods

1. **Download the Mod SDK** — included in every release under `ModSDK/`
2. **Read the modding docs** — see [`/docs/modding`](docs/modding/) or the [Wiki](../../wiki)
3. **Use the example mods** — starter templates are in `ModSDK/examples/`
4. **Test locally** — point the game to your mod folder in `settings.json`
5. **Share your work** — post in [#mod-releases](https://discord.gg/your-invite) on Discord

### Mod Folder Structure

```
my-cool-mod/
├── mod.json          ← Metadata: name, version, author, dependencies
├── assets/
│   ├── textures/
│   ├── sounds/
│   └── models/
├── scripts/          ← Lua scripts for game logic
├── maps/             ← Custom map files (.jwmap)
└── README.md         ← Tell people what your mod does!
```

### `mod.json` Reference

```json
{
  "id": "my-cool-mod",
  "name": "My Cool Mod",
  "version": "1.0.0",
  "author": "YourName",
  "game_version": ">=1.4.0",
  "description": "Adds new weapons and a jungle biome.",
  "dependencies": [],
  "tags": ["weapons", "terrain"]
}
```

---

## 🚀 Installation

### Fresh Install

1. Go to [**Releases**](../../releases) and download the latest stable build for your OS
2. Run the installer (Windows) or extract the archive (Linux/macOS)
3. Launch `JungleWarfair` — no additional setup required

### Installing Mods

1. Download a mod (`.zip` or folder)
2. Extract it into your mods directory:
   - **Windows:** `%APPDATA%\JungleWarfair\mods\`
   - **Linux:** `~/.config/JungleWarfair/mods/`
   - **macOS:** `~/Library/Application Support/JungleWarfair/mods/`
3. Launch the game and enable the mod in **Settings → Mods**
4. Restart if prompted

### Updating

The game will notify you in-app when a new version is available. You can also watch this repo (👁️ **Watch → Releases only**) to get notified on GitHub.

> ⚠️ **Before updating:** Back up your saves and check if your mods are compatible with the new version.

---

## 📋 Changelog

Full patch notes for every version are available in the [Releases](../../releases) tab and in [`CHANGELOG.md`](CHANGELOG.md).

**Recent highlights:**
- `v1.5.0` — New faction system, mod API v2, Linux fixes
- `v1.4.2` — Hotfix: crash on map load with large mod lists
- `v1.4.0` — Procedural terrain overhaul, sound modding support

---

## 🤝 Community & Support

| Resource | Link |
|---|---|
| 💬 Discord | [Join the server](https://discord.gg/your-invite) |
| 🐛 Bug Reports | [Open an issue](../../issues/new?template=bug_report.md) |
| 💡 Feature Requests | [Start a discussion](../../discussions/new?category=ideas) |
| 📖 Wiki & Docs | [Browse the wiki](../../wiki) |
| 🗺️ Mod Showcase | [Show off your mods](../../discussions/categories/mod-showcase) |

Found a bug? Please include your OS, game version, and any mods installed when reporting.

---

## ⚖️ License & Legal

Jungle Warfair is released under the [MIT License](LICENSE).  
You are free to create and distribute mods, including commercial ones, as long as you do not redistribute the base game itself.

- ✅ Creating and selling mods — **allowed**
- ✅ Streaming and making videos — **allowed**  
- ✅ Forking modding tools from this repo — **allowed**
- ❌ Redistributing the game binaries — **not allowed**
- ❌ Removing credits from mods that include original game assets — **not allowed**

---

<div align="center">

Made with 🌿 by the Jungle Warfair team  
*Drop into the canopy. Adapt or die.*

</div>
