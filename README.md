# Velluto i3 – A Luxe i3wm Setup for EndeavourOS

**macOS meets brutalist minimalism**—in warm bronze, cream, and copper.  
Inspired by luxury editorial design, this setup turns i3 into a visual experience.

## ✨ Features

- 🖼 Color-themed with `pywal` and Velluto palette
- 🧱 Polybar with minimal, icon-based layout
- 🔍 Rofi styled like a warm, ambient launcher
- 🌫 Smooth blur and shadows via Picom
- 📦 Easy install with `install.sh`

## 📸 Preview

![Screenshot](wallpaper/velluto-base.jpg)

## 🚀 Installation

```bash
git clone https://github.com/yourusername/velluto-i3 ~/.velluto-i3
cd ~/.velluto-i3
./install.sh

---

## 🛠️ `install.sh` (Basic Setup Script)

```bash
#!/bin/bash

echo "Installing Velluto i3 config..."

mkdir -p ~/.config/i3 ~/.config/polybar ~/.config/rofi ~/.config/picom
cp config/i3/* ~/.config/i3/
cp config/polybar/* ~/.config/polybar/
cp config/rofi/* ~/.config/rofi/
cp config/picom/* ~/.config/picom/
mkdir -p ~/Pictures
cp wallpaper/velluto-base.jpg ~/Pictures/

echo "Done. Log out and back in, or restart i3 to apply."
