# Flustro

Welcome to the official public repository for **Flustro** — The lightning-fast, offline-first voice dictation app that types directly into your cursor on Linux, Windows, and macOS.

> [!NOTE] 
> **The main Flustro source code is private.** This public repository serves three purposes:
> 1. Hosting compiled release binaries (installers) via GitHub Releases.
> 2. Providing a public Issue Tracker for bug reports and feature requests.
> 3. Hosting public Discussions and Community support.

## 🚀 Download Flustro

To get the latest version of Flustro, please visit our official website:
👉 **[https://flustro.app](https://flustro.vercel.app)**

You can also download the raw installer files (`.deb`, `.AppImage`, `.msi`, `.exe`, `.dmg`) directly from the **[Releases Tab](../../releases/latest)**.

## ⚡ Core Features

- 🎙️ **Local-First Privacy**: Runs completely offline using native Moonshine STT or bundled compressed Whisper models. No cloud processing required.
- ⌨️ **Direct Injection**: Press your hotkey (`Ctrl+Space`) to instantly dictate and inject text into any active window across your OS.
- 🧠 **Intelligent Cleanup**: Speak your messy thoughts; Flustro's local Ollama integration formats it perfectly into Code, Emails, Meeting Notes, or Messages.
- 💻 **Cross-Platform**: Natively built using Rust and Tauri v2 for Linux (Wayland/X11), Windows, and macOS.

## 🛠️ Troubleshooting & OS-Specific Fixes

### macOS (Gatekeeper Warning)
Because Flustro is built by an indie developer, macOS might flag the installer as "damaged" because it lacks a paid Apple Developer certificate. 
**To bypass this:**
1. **Right-click** (or Control-click) the Flustro app in your Applications folder.
2. Select **Open**.
3. Click **Open** again in the warning dialog.
*(Alternatively, run `xattr -cr /Applications/Flustro.app` in your Terminal to strip the quarantine flag entirely).*

### Linux (Wayland Users)
Wayland compositors block automated keyboard ghosting for security reasons. Flustro automatically detects Wayland and safely falls back to a clipboard-pasting method to inject your dictations seamlessly. Make sure your system clipboard manager isn't blocking rapid pastes!

## 🐞 Bug Reports & Feedback

We rely on this repository to track feedback from our users.
- Found a bug? [Open an Issue](../../issues/new)
- Have a feature request or question? Join our [Discussions](../../discussions)

---
*Built with ❤️ by [CEYT of eleyoungtech](https://github.com/Codeleyoungtech)*
