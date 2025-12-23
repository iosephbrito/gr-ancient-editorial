# gr-ancient-editorial

An extended Ancient Greek (polytonic) input method for **m17n / fcitx5**,  
designed for **editorial, epigraphic, and scholarly work**.

This project is based on the classic `grc-mizuochi` input method and adds
features required by professional philologists.

---

## Features

- Full polytonic Greek support
- Vowel quantity:
  - Macron (ᾱ ῑ ῡ)
  - Breve (ᾰ ῐ ῠ)
- Combining diacritics for accent stacking
- Lunate sigma (ϲ Ϲ)
- Archaic Greek letters (san, heta, sho)
- Editorial marks (combining dot above/below)
- Compatible with **fcitx5** and **ibus**

---

## Installation (fcitx5)

```bash
mkdir -p ~/.local/share/m17n
cp m17n/grc-ancient-editorial.mim ~/.local/share/m17n/

rm -rf ~/.cache/m17n
fcitx5 -r
