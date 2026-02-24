# VGRD 2.0 — Virus Guard System

> **Browser Threat Detection & Elimination Engine**

![VGRD Banner](https://img.shields.io/badge/VGRD-v2.0-00d4ff?style=for-the-badge&labelColor=03070d)
![License](https://img.shields.io/badge/License-MIT-00ff88?style=for-the-badge&labelColor=03070d)
![HTML](https://img.shields.io/badge/Built_With-HTML%2FJS-ff2d55?style=for-the-badge&labelColor=03070d)
![No Dependencies](https://img.shields.io/badge/Dependencies-ZERO-ffaa00?style=for-the-badge&labelColor=03070d)

---

## 🛡️ What is VGRD?

VGRD (Virus Guard) is a **zero-dependency, single-file browser security scanner** that detects, fixes, and eliminates threats lurking in your browser's JavaScript environment.

It scans the `window` object and page environment for known attack vectors — including API hijacks, crypto miners, malicious iframes, tracking scripts, and more — then gives you the power to **fix or eliminate each threat** with one click.

---

## ✨ Features

| Feature | Description |
|---|---|
| 🔍 **Full Scan** | Runs 10 security checks across your browser environment |
| 🔧 **Fix** | Repairs issues by restoring native browser APIs from a clean context |
| 💀 **Eliminate** | Permanently neutralizes threats by sealing attack vectors |
| ✦ **Fix All** | Batch-fixes every detected issue in one click |
| ✕ **Eliminate All** | Nuclear option — kills all threats simultaneously |
| ⚙️ **Deep Repair** | Restores ALL critical browser APIs and reruns verification scan |
| 📊 **Health Score** | Live integrity score that updates as threats are resolved |
| 🖥️ **System Terminal** | Real-time log of all scan and repair activity |

---

## 🔬 Security Checks Performed

1. **HTTPS Protocol** — Detects unencrypted HTTP connections
2. **eval() Integrity** — Detects if `eval()` has been overridden (malware injection vector)
3. **Console Integrity** — Detects hijacked `console.log()` (keyloggers, debug suppressors)
4. **fetch() Override** — Detects monkey-patched fetch (request interception)
5. **XHR Intercept** — Detects overridden `XMLHttpRequest` (AJAX hijacking)
6. **Crypto Miner Detection** — Scans for known mining libraries (CoinHive, JSEcoin, etc.)
7. **LocalStorage Audit** — Flags sensitive keys that may expose credentials
8. **Cross-Origin Iframes** — Detects potentially malicious embedded frames
9. **Tracker Script Audit** — Identifies external analytics and beacon scripts
10. **MutationObserver Guard** — Detects overridden DOM surveillance observers

---

## 🚀 Live Demo

> **[👉 Try it live on GitHub Pages](https://YOUR-USERNAME.github.io/vgrd)**

---

## 📦 Installation

No installation needed. It's a single HTML file.

**Option 1 — Just open it:**
```bash
git clone https://github.com/YOUR-USERNAME/vgrd.git
cd vgrd
open index.html
```

**Option 2 — Serve locally:**
```bash
npx serve .
# or
python3 -m http.server 8080
```

---

## 🗂️ Project Structure

```
vgrd/
├── index.html        ← Entire application (zero dependencies)
├── README.md         ← This file
├── LICENSE           ← MIT License
└── .github/
    └── workflows/
        └── deploy.yml  ← Auto-deploy to GitHub Pages
```

---

## 🛠️ How It Works

VGRD inspects the browser's `window` object at runtime to detect tampering:

- **Detection** — Each check runs a targeted probe (e.g. `eval.toString().includes('[native code]')`)
- **Fix** — Restores native implementations by cloning them from a sandboxed `<iframe>`
- **Eliminate** — Permanently seals the attack vector using `Object.defineProperty` or function overrides
- **Deep Repair** — Clones ALL native APIs from a fresh iframe context in one pass

---

## 💡 Use Cases

- 🎓 **Security education** — Demonstrate browser-level attack vectors to developers
- 🔒 **Developer tool** — Verify your web app's runtime environment hasn't been tampered with
- 🧪 **Pen testing aid** — Quickly audit a page for signs of client-side compromise
- 📋 **Portfolio piece** — Showcase advanced JavaScript and UI/UX skills

---

## ⚠️ Disclaimer

VGRD scans the **browser JavaScript environment** — it does not scan your operating system, files, or network traffic. It is not a replacement for traditional antivirus software. Use it as a complementary browser-layer security awareness tool.

---

## 📄 License

MIT License — free to use, modify, and distribute. See [LICENSE](LICENSE) for details.

---

## 🙌 Contributing

Pull requests welcome! Ideas for new checks, UI improvements, or browser extension ports are all appreciated.

1. Fork the repo
2. Create your branch: `git checkout -b feature/new-check`
3. Commit: `git commit -m 'Add new security check'`
4. Push: `git push origin feature/new-check`
5. Open a Pull Request

---

<div align="center">
  <strong>Built with 💙 — VGRD 2.0 © 2026</strong>
</div>
