<div align="center">

# 🧭 qutebrowser Configuration
### Keyboard-Driven, Minimalist Vim-Style Web Browsing Environment

[![qutebrowser](https://img.shields.io/badge/qutebrowser-v3.0+-58a6ff?style=flat&logo=qutebrowser&logoColor=white)](https://qutebrowser.org/)
[![Python](https://img.shields.io/badge/Config-Python_3-3776AB?style=flat&logo=python&logoColor=white)](https://www.python.org/)
[![Vim](https://img.shields.io/badge/Navigation-Modal_%7C_Vim_Keybinds-019833?style=flat&logo=vim&logoColor=white)](https://www.vim.org/)
[![Theme](https://img.shields.io/badge/Theme-Dark_Minimal-161b22?style=flat&logo=archlinux&logoColor=white)](https://github.com/5aranx/qutebrowser)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

<br/>

<p align="center">
  <b>A finely tuned, keyboard-first qutebrowser configuration engineered for distraction-free, ultra-low-latency browsing.</b><br/>
  Featuring customized tab behavior, curated quickmarks, persistent security profiles, and custom CSS styling matching modern Linux tiling window managers.
</p>

</div>

---

## 📌 Repository Structure

```
qutebrowser/
├── config.py           # Core Python configuration script and granular engine overrides
├── autoconfig.yml      # Persistent GUI/web-engine state configurations
├── bookmarks/          # Hierarchical bookmark trees
│   └── urls            # Categorized reference URLs
└── quickmarks          # Short-alias instantaneous jump targets (e.g., gh, yt, mail)
```

---

## ✨ Features & Ergonomics

- **True Modal Navigation:** Complete mouseless navigation powered by Vim-standard keybindings (`j/k/h/l` scrolling, `f` hinted link following, `d` tab closing, `o` URL opening).
- **Tailored Visual Styling:** Minimal status bar, hidden window titles, and compact vertical tab bars optimized for tiling window managers (Hyprland, DWM, Sway).
- **Privacy & Telemetry Hardening:**
  - Disabled third-party cookies and aggressive tracker blocking enabled.
  - Native dark-mode rendering injection for reduced eye strain.
  - Granular permissions per-domain for clipboard, geolocation, and media devices.
- **Instantaneous Quickmarks:** Pre-mapped shortcuts for developer docs, GitHub repositories, and system monitoring dashboards.

---

## 🚀 Installation & Deployment

Deploy this configuration into your standard XDG configuration path:

```bash
# Backup existing qutebrowser configuration
mv ~/.config/qutebrowser ~/.config/qutebrowser.bak 2>/dev/null || true

# Clone configuration directly into ~/.config/qutebrowser
git clone https://github.com/5aranx/qutebrowser.git ~/.config/qutebrowser

# Launch qutebrowser
qutebrowser &
```

---

## ⌨️ Essential Keybindings Reference

| Keystroke | Mode | Action |
|---|---|---|
| `o` / `O` | Normal | Open URL in current / new tab |
| `f` / `F` | Normal | Follow link hinted on page in current / background tab |
| `b` / `B` | Normal | Jump to quickmark / Open bookmark |
| `d` | Normal | Close active tab |
| `u` | Normal | Undo last closed tab |
| `gt` / `gT` | Normal | Next tab / Previous tab |
| `gi` | Normal | Focus first input text field on page |
| `:set <key>` | Command | Real-time setting override without restarting browser |

---

## 📄 License

This configuration is open source and available under the [MIT License](LICENSE).

---

<div align="center">
  <sub>Configured for maximum ergonomics and terminal workflow synergy.</sub><br/>
  <b>Made by Saransh Singh</b>
</div>
