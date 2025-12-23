# gr-ancient-editorial

An extended Ancient Greek (polytonic) input method for **m17n / fcitx5**,  
designed for **editorial, epigraphic, and scholarly work**.

This project is based on the classic `grc-mizuochi` input method from the
m17n database and extends it with features required by professional
philologists, linguists, and classicists.

---

## Features

- Full polytonic Greek support
- Vowel quantity:
  - Macron (ᾱ ῑ ῡ)
  - Breve (ᾰ ῐ ῠ)
- Combining diacritics for accent stacking
- Lunate sigma (ϲ Ϲ) for papyrology and epigraphy
- Archaic Greek letters (san, heta, sho)
- Editorial marks:
  - combining dot below
  - combining dot above
- Unicode-compliant
- Works with **fcitx5** and **ibus**

---

## Installation (fcitx5)

```bash
mkdir -p ~/.local/share/m17n
cp m17n/grc-ancient-editorial.mim ~/.local/share/m17n/

rm -rf ~/.cache/m17n
fcitx5 -r
````

After restarting, add the input method in fcitx5:

```
Greek → ancient-editorial
```

---

## Basic usage examples

| Keys | Output | Description         |
| ---- | ------ | ------------------- |
| `a=` | ᾱ      | alpha with macron   |
| `a_` | ᾰ      | alpha with breve    |
| `i=` | ῑ      | iota with macron    |
| `sc` | ϲ      | lunate sigma        |
| `.`  | ◌̣     | combining dot below |
| `=`  | ◌̄     | combining macron    |

Accents stack normally using combining marks:

```
a=/'  → ᾱ́
```

---

## Background

The original **Mizuochi** input method provides excellent coverage of
polytonic Greek but does not include certain features required in
critical editions, grammars, lexica, and epigraphic work.

This project extends it while preserving:

* original key logic
* muscle memory
* compatibility with existing workflows

---

## Compatibility

* Tested with:

  * fcitx5 + m17n
* Should work with:

  * ibus-m17n
* No patches to m17n itself required

---

## License

This project is licensed under the **GNU Lesser General Public License
v2.1 or (at your option) any later version**.

It is a derivative work of:

* `grc-mizuochi.mim`

  * © 2006–2008 National Institute of Advanced Industrial Science and Technology (AIST)

Modifications and extensions:

* © 2025

See the `LICENSE` file for the full license text.

```

---

### ✅ Tip to avoid GitHub truncation again
When pasting:
- Use **one continuous paste**
- Avoid switching editor tabs mid-paste
- Prefer GitHub’s **“Edit file → raw markdown”** view

---

If you want next, I can:
- tailor the README for **submission to m17n-db**
- add a **Key Reference table** section
- write a short **ANNOUNCE.md** for release tagging

You’re very close to a polished first release.
```
