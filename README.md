# free-panorama

**Fully open `code.pbin` for CS:GO — no packing or unpacking required.**

---

## 📖 About

`free-panorama` is an open alternative to the standard `code.pbin` for Counter-Strike: Global Offensive.

A regular `code.pbin` is a **packed archive**: the entire interface (`panorama/`, `layout/`, `styles/`, `scripts/`, etc.) lives *inside* the file. To change anything, you have to unpack the `.pbin`, edit the files, and repack it — every single time.

`free-panorama` solves this: it is **not a panorama and not an archive**, but a **connector**. All interface files sit **right next to** `code.pbin` as ordinary folders and files. The game reads them directly — no packing, unpacking, or rebuilding.

---

## ✨ Features

- 🔓 **Fully open** — sources are available; inspect and modify anything.
- 📂 **No packing/unpacking** — all interface files live next to `code.pbin` in plain form.
- 🧩 **`code.pbin` as a connector** — the file does not contain the panorama inside itself; it only redirects the game to the files alongside it.
- ⚡ **Fast iteration** — edit a file and see the result in-game immediately, with no archive rebuild.
- 🛠️ **Modding-friendly** — perfect for custom HUDs, interface skins, and experiments.

---

## 📁 Structure
csgo/
└── panorama/
├── code.pbin ← connector (contains no files inside)
├── layout/ ← interface files live alongside
├── styles/
├── scripts/
