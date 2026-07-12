# 🗂️ RecollectViewer

[![Platform](https://img.shields.io/badge/Platform-Windows%2010%20%2F%2011-blue)](https://www.yasui-kamo.com/labo/recollectviewer/)
[![.NET Framework](https://img.shields.io/badge/.NET%20Framework-4.7.2+-512BD4)](https://dotnet.microsoft.com/)
[![Latest release](https://img.shields.io/github/v/release/y-tomioka/RecollectViewer?label=release)](https://github.com/y-tomioka/RecollectViewer/releases)

**Find any past AI conversation in seconds — completely offline.**

RecollectViewer is a free Windows desktop app that loads exported chat history from **ChatGPT, Gemini, and Claude**, then lets you browse it in a tree view and search across everything with powerful filters. Your data never leaves your PC.

⭐ **If you find this app helpful, please give this repository a Star!** ⭐

> 🌐 **Official product page (Japanese, with full tutorials):**  
> https://www.yasui-kamo.com/labo/recollectviewer/

---

## 📦 About this repository

This repository distributes **pre-built binaries only**. Source code is not published here.

- 📥 **Download:** [GitHub Releases](https://github.com/y-tomioka/RecollectViewer/releases)

> 💡 For a lightweight open-source edition (Gemini tree view only), see [RecollectViewerLite](https://github.com/y-tomioka/RecollectViewerLite).

---

## 📸 Screenshots

<table>
  <tr>
    <td align="center" width="50%"><b>Unified tree</b></td>
    <td align="center" width="50%"><b>Cross-AI search</b></td>
  </tr>
  <tr>
    <td align="center" width="50%">
      <img src="https://github.com/user-attachments/assets/550a3b4f-7ef9-4a1e-a802-b415b4de6473" alt="Unified tree view" width="100%" />
    </td>
    <td align="center" width="50%">
      <img src="https://github.com/user-attachments/assets/da9458fb-5ea0-4532-8875-b87184b0164f" alt="Cross-AI search" width="100%" />
    </td>
  </tr>
</table>


---

## 💡 Why RecollectViewer?

- *"Where did that code snippet go that the AI wrote for me?"*
- *"I'm sure I already solved this — which chat was it in?"*

If you use more than one AI service, your conversation history is scattered across exports and formats. RecollectViewer brings it together in one window so you can **browse, search, and jump back to the exact exchange** — without uploading anything to the cloud.

---

## ✨ Key features

### 🌳 Unified browsing
- **ChatGPT** — month → chat → conversation blocks
- **Gemini** — year → month → day (organized by date)
- **Claude** — month → chat → conversation blocks

### 🔍 Cross-AI full-text search
Search all loaded history at once. Multiple space-separated keywords work as **AND** conditions.

### ⚙️ Advanced search (7 filters)
Combine these with your keywords:

| Filter | Options |
| :--- | :--- |
| **Search scope** | Prompt & response · Prompt only · Response only |
| **Target AI** | All · ChatGPT · Gemini · Claude |
| **Contains code** | Code blocks only |
| **Contains files/images** | Chats with attachments or generated images |
| **Date range** | Start / end date |
| **Exclude keyword** | NOT filter |

### 📖 Reading experience
- Markdown rendering with tables
- Syntax highlighting for major programming languages
- One-click **Copy** on code blocks
- Open bundled attachments directly from the chat view
- Jump from search results to the matching tree node

### 🔒 Privacy
- **100% offline** — no network calls while using the app
- Safe for confidential or personal chat exports

### 🌍 Localization
RecollectViewer ships with **English** and **Japanese** UI.
- Japanese Windows → Japanese UI
- Other locales → English UI (fallback)
- Override anytime: set environment variable `RECOLLECTVIEWER_LOCALE` to `en`, `ja`, etc.

---

## 🚀 Quick start

### 1. Download and run
1. Get the latest ZIP from [Releases](https://github.com/y-tomioka/RecollectViewer/releases).
2. Extract the folder anywhere you like (portable — no installer).
3. Run `RecollectViewer.exe`.

> **Requirements:** Windows 10 / 11, .NET Framework 4.7.2+, [WebView2 Runtime](https://developer.microsoft.com/microsoft-edge/webview2/).

### 2. Export your chat data
You need official export files from each AI service:

| Service | Export |
| :--- | :--- |
| **ChatGPT** | Settings → Data controls → Export data |
| **Gemini** | [Google Takeout](https://takeout.google.com/) → My Activity → Gemini app → JSON |
| **Claude** | Settings → Privacy → Export data |

### 3. Load data in the app
1. Open **Settings** from the menu.
2. Point to each service’s JSON file or folder.
3. Paths are saved automatically on next launch.

### 4. Browse or search
- **Tree tab** — expand the hierarchy and pick a conversation.
- **Search tab** — enter keywords, optionally open **Advanced Search Filters**, then press Enter.

---

## ⚠️ Known limitations

RecollectViewer follows each provider’s export format. Please note:

1. **ChatGPT branches** — When a chat was edited, only one representative linear path is shown.
2. **Attachments** — Files open only when the export archive actually includes them.
3. **Claude attachments** — Not included in Claude’s official export (preview/search not supported).
4. **Gemini threading** — Takeout data has no stable chat-thread IDs, so history is grouped **by date**.

---

## 👨‍💻 About the Developer

Developed by a solo engineer passionate about building robust, offline-first Windows utilities. 

---

## 📰 Media coverage
Featured on major Japanese software portals:
- [窓の杜 (Impress Watch) — v1.0 / v1.2](https://forest.watch.impress.co.jp/docs/digest/2104593.html) (Jul 2026)
- [フリーソフト100 — v1.1 review](https://freesoft-100.com/review/recollectviewer.html) (May 2026)
- **Intro video:** [YouTube](https://www.youtube.com/watch?v=dbkoX5j2PDA)

---

## 📄 Terms of use
RecollectViewer is free for personal and commercial use.
**Prohibited:** using the software to view, monitor, or analyze **other people’s** chat data without permission. The software is provided **as-is** without warranty.

---

## 🗑️ Uninstall
Delete the extracted folder. No registry entries are created.
