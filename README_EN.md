# Batch Rename Pro for After Effects

[![License](https://img.shields.io/badge/License-No%20commercial%20use-blue.svg)](./LICENSE)
[![Language](https://img.shields.io/badge/Language-7%20Languages-green.svg)](#language-support)

**Batch Rename Pro** is a powerful batch renaming script for Adobe After Effects. It supports items in the Project panel as well as layers in the current composition's timeline, offering four renaming modes: **Format Rename**, **Text Replace**, **Add Sequence**, and **Add Text**. The interface is clean, multilingual, and remembers your settings.

> **Author**: ZBT Studio  
> **Code**: Fully written by [DeepSeek](https://chat.deepseek.com/)

---

## ✨ Features

- 🎯 **Four Renaming Modes**
  - **Format Rename**: Batch define base name + sequence (prefix/suffix)
  - **Replace Text**: Find and replace any text in the name
  - **Add Sequence**: Append an incremental sequence number to the original name (prefix/suffix)
  - **Add Text**: Insert custom text at the beginning or end of the name

- 🌐 **Multi-language Support** (7 built-in languages, switch anytime)
  - 简体中文 · English · Français · Italiano · Русский · 日本語 · 한국어

- 🖱️ **Friendly Interaction**
  - Each mode has its own independent parameter panel

- 💾 **Persistent Settings**
  - Automatically saves your configuration

- 📁 **Flexible Target Selection**
  - Supports any selected items in the **Project** panel (files, comps, folders, etc.)
  - Supports selected layers in the **current composition's Timeline** (ordered by layer order)

- 📜 **Copyright & Author Info**
  - For learning purposes only. You may modify, copy, and redistribute freely, but **commercial use is strictly prohibited**.

---

## 🚀 Usage

### Installation
1. Go to the [release](https://github.com/zbt00123/Batch-Rename-Pro-for-AE/releases/tag/AE_Scripts) page to download the `Batch Rename Pro for AE.jsx` script file.
2. Place it in the After Effects script directory:
   - Windows: `C:\Program Files\Adobe\Adobe After Effects <version>\Support Files\Scripts\ScriptUI Panels\`
   - macOS: `/Applications/Adobe After Effects <version>/Scripts/ScriptUI Panels/`
3. In After Effects, open the panel via `Window` > `Batch Rename Pro.jsx`.

### Basic Operations
1. Select items in the **Project** panel, or select layers in the **current composition's timeline**.
2. In the script panel, choose a renaming **mode** (Format / Replace / Add Sequence / Add Text).
3. Fill in the parameters according to the mode (e.g., base name, separator, start number, etc.).
4. Click the **"Execute Rename"** button.

> **Note**: The operation creates an undo step (`Undo`). If you're not satisfied with the result, press `Ctrl+Z` (Win) or `Cmd+Z` (Mac) to undo.

---

## ⚙️ Mode Parameter Description

| Mode | Parameters | Description |
|------|------------|-------------|
| **Format Rename** | Base name, Separator, Start, Step, Digits, Sequence position | Generates `BaseName_Sequence` or `Sequence_BaseName` format, with sequence incrementing as set |
| **Replace Text** | Find, Replace with | Replaces all occurrences of specified text in the name with new text |
| **Add Sequence** | Separator, Start, Step, Digits, Sequence position | Appends an incremental sequence to the original name (suffix or prefix), e.g., `OriginalName_001` |
| **Add Text** | Text to add, Position (beginning/end) | Inserts fixed text at the beginning or end of the name |

- **Sequence position**: `Suffix` means the sequence is at the end, `Prefix` means at the beginning.
- **Start / Step / Digits**: Supports mouse wheel, up/down buttons, and keyboard arrow keys for quick adjustment.

---

## 🌐 Language Switching

Click the **⚙** gear button on the main panel to open the settings window, then select your preferred language from the **Language** dropdown. The language setting is saved automatically and will be applied the next time you open the script.

---

## 📝 Notes

- The script only affects **items selected in the Project window** or **layers selected in the current composition's timeline**; no other objects are touched.
- If both project items and timeline layers are selected, the script prioritizes the **Project window selection** (matching After Effects' default behavior).
- If the "Find" field in Replace mode is empty, the script will display an error.
- It is recommended to keep the number of digits between 1 and 10. Start and Step values are range‑limited (0–999999 and 1–999999 respectively); out‑of‑range values will trigger a warning.

---

## 📄 License

This script is **for learning purposes only**. You are free to modify, copy, and redistribute it, but **commercial use is strictly prohibited**.  
For the full license text, please refer to the copyright information inside the script (also viewable in the settings window).

---

## 🤝 Contributions & Feedback

Issues and Pull Requests are welcome at [GitHub](https://github.com/zbt00123/Batch-Rename-Pro-for-AE).  
If you find any problems or have suggestions for improvement, please open an issue in the repository.

---

## 🙏 Acknowledgements

- Thanks to **DeepSeek** for providing powerful AI coding support.
- Thanks to all users and testers of this script.
