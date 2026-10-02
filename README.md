# Trim Press Tonnage Calculator

**Live demo:** https://zov911.github.io/trim-press-tonnage-calculator/

Calculates the trimming and blanking force for die castings, forgings and sheet metal, then recommends a press capacity class. Results update live in US or metric units.

## Features

- **21 materials in 3 categories plus custom:**
  - *Die-cast:* A380/ADC12, A360, structural HPDC (AlSi10MnMg), Zamak 3, Zamak 5, ZA-8, AZ91D magnesium
  - *Sheet & plate:* aluminum 1100/5052/6061, copper, brass, mild steel, HSLA, stainless 304/316, AHSS DP600/DP980
  - *Forgings:* steel hot trim, steel cold trim, aluminum
  - *Custom:* enter any shear strength in MPa or ksi
- **One source of truth for material data:** shear strength is stored in MPa, so US and metric results always agree
- **Trim-line shapes:** round, square, rectangle, slot, or a custom/CAD perimeter, plus extra cut length for holes, gates and overflows
- **Die factors:** parts per stroke (multi-cavity), stripping allowance and safety margin
- **Press class recommendation** from standard capacities (10–1,600 t), targeting ≤ 80% working load
- **Engineering notes** for the selected material: gate breakout, hot-trim temperature sensitivity, AHSS snap-through and clearance, hydraulic vs mechanical tonnage curves, off-center loading
- Copy summary, shareable links, print, and a mobile layout

## Method

```
F = cut length × thickness × shear strength × parts per stroke × (1 + stripping) × (1 + safety margin)
```

Results are given in kN, US tons and metric tonnes. Shear strengths are typical room-temperature handbook values (hot-trim values are approximate). Use certified material data and press-builder review for final design.

## Tech

A single self-contained `index.html`: vanilla HTML, CSS and JavaScript with no build step and no dependencies (Google Fonts only).

---

## Want this calculator for your business?

I build custom engineering calculators and product configurators for press builders, die shops and foundries. They match your machines and brand, and send qualified quote requests to your sales team.

**Reach out → [zov911.com](https://zov911.com)**

© 2026 zov911. All rights reserved.
