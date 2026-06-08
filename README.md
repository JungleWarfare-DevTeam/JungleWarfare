<div align="center">

```
     ██╗██╗   ██╗███╗  ██╗ ██████╗ ██╗     ███████╗
     ██║██║   ██║████╗ ██║██╔════╝ ██║     ██╔════╝
     ██║██║   ██║██╔██╗██║██║ ███╗ ██║     █████╗
██   ██║██║   ██║██║╚████║██║  ██║ ██║     ██╔══╝
╚█████╔╝╚██████╔╝██║ ╚███║╚██████║ ███████╗███████╗
 ╚════╝  ╚═════╝ ╚═╝  ╚══╝ ╚═════╝ ╚══════╝╚══════╝

██╗    ██╗ █████╗ ██████╗ ███████╗ █████╗ ██████╗ ███████╗
██║    ██║██╔══██╗██╔══██╗██╔════╝██╔══██╗██╔══██╗██╔════╝
██║ █╗ ██║███████║██████╔╝█████╗  ███████║██████╔╝█████╗
██║███╗██║██╔══██║██╔══██╗██╔══╝  ██╔══██║██╔══██╗██╔══╝
╚███╔███╔╝██║  ██║██║  ██║██║     ██║  ██║██║  ██║███████╗
 ╚══╝╚══╝ ╚═╝  ╚═╝╚═╝  ╚═╝╚═╝     ╚═╝  ╚═╝╚═╝  ╚═╝╚══════╝
```

**Build. Command. Raid. Survive.**  
*A jungle survival war game — with a full modding framework.*

[![Latest Release](https://img.shields.io/github/v/release/JungleWarfare-DevTeam/JungleWarfare?style=for-the-badge&color=3a6b35&label=Latest+Release)](../../releases/latest)
[![Downloads](https://img.shields.io/github/downloads/JungleWarfare-DevTeam/JungleWarfare/total?style=for-the-badge&color=2d5016&label=Total+Downloads)](../../releases)
[![Godot 4.x](https://img.shields.io/badge/Godot-4.x-478cbf?style=for-the-badge&logo=godotengine&logoColor=white)](https://godotengine.org/)
[![GDScript](https://img.shields.io/badge/Mods-GDScript-478cbf?style=for-the-badge)](https://docs.godotengine.org/en/stable/tutorials/scripting/gdscript/)
[![Source Code](https://img.shields.io/badge/Source_Code-Closed-red?style=for-the-badge)]()
[![License](https://img.shields.io/badge/License-Proprietary-lightgrey?style=for-the-badge)](LICENSE)

</div>

---

> **What is this repo?**  
> This is the official **releases page** for Jungle Warfare — game binaries and the Mod SDK are both distributed here.  
> The game is **free to download and play**. The **source code is closed and will not be made available** under any circumstances.  
> Do not open issues or pull requests asking for source access — those will be closed without response.

---

## 📑 Table of Contents

- [About the Game](#about-the-game)
- [Dedicated Servers & Anti-Cheat](#dedicated-servers--anti-cheat)
- [Downloads](#downloads)
  - [Installing the Game](#installing-the-game)
  - [Setting Up a Dedicated Server](#setting-up-a-dedicated-server)
  - [Mod SDK Contents](#mod-sdk-contents)
- [Modding](#️-modding)
  - [Prerequisites](#prerequisites)
  - [Mod Folder Structure](#mod-folder-structure)
  - [Naming Rules](#naming-rules)
  - [manifest.json](#manifestjson)
  - [Supported Asset Types](#supported-asset-types)
  - [Avoiding Conflicts with Other Mods](#avoiding-conflicts-with-other-mods)
  - [Available Autoloads](#available-autoloads)
  - [GameEvents Signals](#gameevents-signals)
  - [Building Your Mod](#building-your-mod)
  - [Installing a Mod on a Server](#installing-a-mod-on-a-server)
- [Troubleshooting](#troubleshooting)
- [Versioning](#versioning)
- [Changelog](#changelog)
- [Sharing Your Mod](#sharing-your-mod)
- [License](#license)

---

## 🎮 About the Game

**Jungle Warfare** is a multiplayer survival war game set in dense, hostile jungle. Think Rust — but deeper in the canopy, and with an RTS twist.

- 🪵 **Build like Rust** — gather resources, construct and fortify your base in the jungle
- 🪖 **Command troops** — direct AI soldiers to raid, defend, and flank enemy positions
- ⚔️ **Raid other players** — knock down their bases, take their resources, dominate the map
- 🌿 **The jungle is the third enemy** — terrain, wildlife, and visibility all work against you
- 🖥️ **Dedicated servers only** — no peer-to-peer, no local hosting, no offline play
- 🥽 **VR support** — a full VR client is available alongside the standard client
- 🚫 **Zero tolerance for cheating** — see the server rules below

> There is no save system. What you build, you defend. What you lose, you lose.

---

## 🖥️ Dedicated Servers & Anti-Cheat

Jungle Warfare runs exclusively on dedicated servers. There are no peer-to-peer options.

**How mods work in multiplayer:**  
Mods are installed on the server, not the client. When a player connects, the server automatically sends all active mods to their client. Players never need to manually download or install mods — it just works.

**Server rules are strictly enforced by the Jungle Warfare Dev Team:**

- Cheating, exploiting, or using modified clients to gain an unfair advantage results in a **permanent ban**
- Mods are distributed server-to-client automatically and run in a sandboxed environment — clients cannot inject unauthorised code
- Mods cannot access internals outside the published mod API

> ⚠️ **Mods are for server customisation, not client advantage.**  
> If your mod gives one player an edge that others can't see or counter, it won't be allowed on any official server.

---

## 📦 Downloads

### [⬇️ Go to Releases →](../../releases/latest)

All official releases are published here by the Jungle Warfare Dev Team:

| Download | Who it's for |
|---|---|
| 🎮 **Game Client** (`.exe` / `.AppImage` / `.dmg`) | Players who want to connect to servers and play |
| 🥽 **VR Client** (`.exe` / `.AppImage` / `.dmg`) | Players with a VR headset |
| 🖥️ **Dedicated Server** (`.exe` / `.AppImage` / `.dmg`) | Anyone who wants to host their own server |
| 🛠️ **Mod SDK** (`.zip`) | Modders who want to build mods for their server |

**Supported platforms:** Windows, Linux, macOS — across all releases

> 🔒 **The source code is not included in any release and is not publicly available.**  
> The binaries are the only form in which the game is distributed.

### Installing the Game

1. Download the client for your platform from [Releases](../../releases/latest)
2. Run the installer (Windows) or extract the archive (Linux/macOS)
3. Launch Jungle Warfare and connect to a server — no account or setup required

> There is no offline mode and no save system. Progress lives on the server.

### Setting Up a Dedicated Server

1. Download the dedicated server package for your platform from [Releases](../../releases/latest)
2. Extract the archive and run `JungleWarfare-Server`
3. Edit `server.cfg` to set your server name, player limit, and other options
4. Drop any `.pck` mod files into the `mods/` folder before starting
5. Forward the required ports and share your server address with players

Players connecting to your server will **automatically receive all server-side mods** — they do not need to install anything manually. See the [Modding](#️-modding) section for how to build mods.

### Mod SDK Contents

Each SDK release includes:

| File | What it is |
|---|---|
| `build_mod.py` | Packs your mod folder into a `.pck` file |
| `read_pck.py` | Inspects a `.pck` to verify its contents |
| `tutorial_mod/` | A fully commented starter mod — read it, it's the tutorial |
| `CHANGELOG.md` | What changed in this SDK version |

SDK releases are versioned alongside the game. Check the release notes to confirm compatibility.

---

## 🛠️ Modding

Jungle Warfare's modding framework is built on **Godot 4** and **GDScript**. Mods are packed into Godot `.pck` files, installed on the server, and automatically delivered to players when they connect. You do **not** need the game source code — the Mod SDK is self-contained.

### Prerequisites

| Tool | Why you need it |
|---|---|
| **Python 3.x** | To run `build_mod.py` (packer) and `read_pck.py` (inspector) |
| **Godot 4.x** | To edit and preview mod scenes and scripts — not required, but strongly recommended |
| A code editor | Any editor works — VS Code with the GDScript extension is a good choice |

---

### Mod Folder Structure

```
my_mod/
├── manifest.json          ← Required: mod metadata (id, name, version, description)
├── mod_main.gd            ← Entry point — runs when your mod loads on the server
├── tools/
│   └── my_tool.gd         ← Custom tools (extend the base tool class)
├── entities/
│   └── my_entity.tscn     ← Spawnable entities (Godot scenes)
├── sounds/
│   └── my_sound.ogg       ← Audio assets
└── icons/
    └── my_tool.png        ← Icons shown in server UI / HUD
```

When packed, all assets are available at runtime under `res://mods/<your_mod_id>/`.

---

### Naming Rules

Mod IDs and **all filenames** must use lowercase letters, numbers, and underscores only:

```
my_jungle_mod   ✓
MyJungleMod     ✗  (no capitals)
my-jungle-mod   ✗  (no hyphens)
```

---

### manifest.json

```json
{
  "id":          "my_mod",
  "name":        "My Mod",
  "version":     "1.0.0",
  "author":      "YourName",
  "description": "What does your mod do?"
}
```

The `id` field must exactly match your mod's folder name. `author` is optional but encouraged.

---

### Supported Asset Types

| Type | Formats | Folder |
|---|---|---|
| Scripts | `.gd` | Anywhere in the mod folder |
| Scenes / entities | `.tscn` | `entities/` |
| Audio | `.ogg` | `sounds/` |
| Icons / textures | `.png` | `icons/`, `textures/` |

Other formats (`.wav`, `.jpg`, `.tres`, `.res`) may work but are untested — stick to the list above.

---

### Avoiding Conflicts with Other Mods

Always prefix your registered IDs with your mod ID:

```gdscript
ToolRegistry.register("my_mod:my_tool", ...)    # ✓ good
ToolRegistry.register("my_tool", ...)           # ✗ bad — may clash with another mod
```

This applies to `ToolRegistry`, `EntityRegistry`, `Console` commands, and any global keys.

---

### Available Autoloads

These are always available in your GDScript:

| Autoload | What it does |
|---|---|
| `ModLoader` | Check if other mods are loaded |
| `ToolRegistry` | Register and look up tools |
| `EntityRegistry` | Register and look up spawnable entities |
| `GameEvents` | Connect to game-wide signals |
| `Console` | Register commands, print to the in-game console |
| `HUD` | Show hints, crosshairs, and notifications |
| `Audio` | Play sounds in 2D or 3D space |

### GameEvents Signals

| Signal | When it fires |
|---|---|
| `player_joined(player)` | A player joins the server |
| `player_left(player)` | A player disconnects |
| `map_changed(map_id)` | The map changes |

---

### Building Your Mod

Run the packer from the SDK folder:

```
python build_mod.py
```

You'll be prompted for:

```
Mod name:         my_mod
Source directory: C:\projects\my_mod    ← the folder containing manifest.json
Output directory: ./dist                ← where to save the .pck
Godot version:    4.2
```

To verify the output before deploying:

```
python read_pck.py
```

All paths inside the `.pck` should start with `res://mods/<your_mod_id>/`. If they don't, you pointed the builder at the wrong folder.

---

### Installing a Mod on a Server

Drop the `.pck` into the server's mods folder:

- **Windows:** `%APPDATA%\JungleWarfare\mods\`
- **Linux / macOS:** `~/.local/share/JungleWarfare/mods/`

Restart the server. Connecting clients will receive the mod automatically — no action needed on the player's side. The `[ModLoader]` lines in the server log will confirm whether the mod loaded successfully.

---

## 🐛 Troubleshooting

**Mod not recognised by the server**
- `manifest.json` must be at the **root** of your mod folder, not inside a subfolder
- Required fields: `id`, `name`, `version`, `description` — all must be present
- The `id` field must exactly match your folder name, lowercase and underscores only
- Double-check the `.pck` is in the correct mods folder for your OS (see above)

**Assets not loading (missing textures, sounds, scenes)**
- Run `python read_pck.py` — paths must start with `res://mods/<your_mod_id>/`
- Make sure you pointed `build_mod.py` at the folder that *contains* `manifest.json`, not a parent folder
- Filenames are case-sensitive on Linux — use lowercase everywhere

**Script errors or mod crashes on load**
- Confirm `mod_main.gd` extends the correct base class — check the tutorial mod for the signature
- If you extended a framework class, make sure the `.pck` was built against a matching Godot version; rerun `build_mod.py` and enter the correct version when prompted
- Check the server log for `[ModLoader]` lines — they will describe exactly what failed

**`build_mod.py` fails or outputs an empty `.pck`**
- Confirm you are running Python 3 (`python3 --version`)
- The source directory must contain `manifest.json` at its root
- On Windows, use a full absolute path with no trailing slash (e.g. `C:\projects\my_mod`)

**ID conflicts with another mod**
- Prefix all registered IDs with your mod ID (see above)
- Use `ModLoader.is_mod_loaded("other_mod_id")` to check before registering shared resources

---

## 🔢 Versioning

Jungle Warfare releases follow **Semantic Versioning** — every release is numbered `vMAJOR.MINOR.PATCH`.

| Number | Changes when... | Example |
|---|---|---|
| **MAJOR** | A huge update — new core game systems, or breaking changes to the mod API | `v1.0.0` → `v2.0.0` |
| **MINOR** | New features, new content, or new mod API additions that don't break existing mods | `v1.3.0` → `v1.4.0` |
| **PATCH** | Bug fixes and hotfixes only — nothing new, nothing broken | `v1.4.1` → `v1.4.2` |

**Rules:** when MAJOR increases, MINOR and PATCH reset to `0`. When MINOR increases, PATCH resets to `0`.

> Releases marked `v0.x.x` are **early access** — the game is still in active development. The `v1.0.0` milestone marks full launch.

If you are a modder, pay attention to MAJOR bumps — these may require updates to your mod to stay compatible. MINOR and PATCH releases will not break existing mods.

---

## 📋 Changelog

Full SDK release notes are in the [Releases](../../releases) tab and in [`CHANGELOG.md`](CHANGELOG.md).

---

## 📢 Sharing Your Mod

There's no central mod store yet — for now, open a [Discussion](../../discussions) in this repo to share your work, get feedback, or find collaborators. The Jungle Warfare Dev Team will share more information on this as the game develops.

---

## ⚖️ License

**The game itself is proprietary and closed source.** The binaries are free to download and play, but you may not decompile, reverse engineer, or redistribute them.

The Mod SDK tooling (`build_mod.py`, `read_pck.py`, and related scripts) is released under the [MIT License](LICENSE) — you are free to fork and modify the tools.

**Summary:**

- ✅ Downloading and playing the game — allowed
- ✅ Creating and sharing mods — allowed
- ✅ Forking and modifying the Mod SDK tooling — allowed
- ❌ Redistributing game binaries — not allowed
- ❌ Decompiling or reverse engineering the game — not allowed
- ❌ Requesting or expecting source code access — will not happen
- ❌ Using mods to bypass anti-cheat or gain unfair advantages — not allowed, results in a permanent ban

---

<div align="center">

*More info coming as development continues — Jungle Warfare Dev Team*

</div>
