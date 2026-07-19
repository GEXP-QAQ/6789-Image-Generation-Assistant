# ⚡ 6789 Image Generation Assistant

**Generate images directly in Codex using Google and GPT image models.**

A fast and flexible image-generation skill featuring a **visual parameter panel**, **configurable generation settings**, and **high-concurrency processing**.

## 📦 Download & Install

[![Download Skill](https://img.shields.io/badge/Download-v1.0.0-2ea44f?style=for-the-badge&logo=github)](https://github.com/GEXP-QAQ/6789-Image-Generation-Assistant/raw/refs/heads/main/relay-image-generator-v1.0.0.zip)
[![View Repository](https://img.shields.io/badge/View-Repository-181717?style=for-the-badge&logo=github)](https://github.com/GEXP-QAQ/6789-Image-Generation-Assistant)

### 🍎 Quick Install for macOS / Linux

Run the following command in Terminal:

```bash
tmp=$(mktemp) && curl -fL "https://github.com/GEXP-QAQ/6789-Image-Generation-Assistant/raw/refs/heads/main/relay-image-generator-v1.0.0.zip" -o "$tmp" && mkdir -p "$HOME/.codex/skills" && rm -rf "$HOME/.codex/skills/relay-image-generator" && unzip -q "$tmp" -d "$HOME/.codex/skills" && rm -f "$tmp"
```

### 🪟 Quick Install for Windows

Run the following commands in PowerShell:

```powershell
$zip = Join-Path $env:TEMP "relay-image-generator-v1.0.0.zip"
$dest = Join-Path $env:USERPROFILE ".codex\skills"
Invoke-WebRequest -Uri "https://github.com/GEXP-QAQ/6789-Image-Generation-Assistant/raw/refs/heads/main/relay-image-generator-v1.0.0.zip" -OutFile $zip
New-Item -ItemType Directory -Force -Path $dest | Out-Null
Remove-Item -Recurse -Force (Join-Path $dest "relay-image-generator") -ErrorAction SilentlyContinue
Expand-Archive -Path $zip -DestinationPath $dest -Force
Remove-Item $zip -Force
```

After installation, **restart Codex** and invoke:

```text
$relay-image-generator
```

<details>
<summary><strong>🖱️ Manual Installation</strong></summary>

1. Click **Download Skill** above.
2. Extract the downloaded ZIP file.
3. Move the `relay-image-generator` folder into:
   - **macOS / Linux:** `~/.codex/skills/`
   - **Windows:** `%USERPROFILE%\.codex\skills\`
4. Restart Codex.

</details>

## 🚀 Quick Start

Invoke the skill directly in Codex:

**`$relay-image-generator`**

<img width="1480" height="76" alt="Invoke relay-image-generator in Codex" src="https://github.com/user-attachments/assets/aa92a341-1958-42fd-8e33-41dce01c375f" />

## 🎛️ Visual Parameter Panel

**Use the right-side control panel to switch models, aspect ratios, image sizes, and other generation settings.**

The panel opens before generation, allowing you to review and adjust parameters easily.

<img width="808" height="1266" alt="Image generation parameter panel" src="https://github.com/user-attachments/assets/2751a820-276b-4ab0-8c34-a9224854cf9d" />

## ⚡ High-Concurrency Generation

**Generate up to 50 images concurrently in a single request.**

Concurrent processing significantly reduces waiting time when generating multiple images.

<img width="1766" height="1422" alt="Concurrent image generation results" src="https://github.com/user-attachments/assets/3bf2e19e-e308-49e0-99f9-07e31209c1d5" />

## 🤖 Supported Models

- **Google image models**
- **GPT image models**
- **Models available through the 6789API relay**

## ✨ Key Features

- 🎛️ **Visual parameter control panel**
- 🖼️ **Up to 50 concurrent image generations**
- ⚙️ **Automatic parameter loading**
- 💾 **Direct image saving**
- 👀 **Inline image previews**
- ⏱️ **Reduced generation waiting time**
- 🪙 **Optimized token usage**
