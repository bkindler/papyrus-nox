# Papyrus Nox — Theme Demo

This file showcases every visual element of the theme. Open it in **Obsidian** with Papyrus Nox enabled to see the full effect.

---

## Headings

### Third-level heading
#### Fourth-level heading
##### Fifth-level heading
###### Sixth-level heading

---

## Body Text & Inline Formatting

The typeface is set in **DM Sans** at a narrow 95 % font-stretch — compact yet readable on screens of any size. The page width is capped at 550 px so your eyes never have to travel far.

You can write **bold text** to highlight key terms, use *italic text* for emphasis, or combine ***both*** when something really matters. ~~Strikethrough~~ works too. Inline `code snippets` stand out with a gold tint on a dark backdrop.

Here is a [link to Obsidian](https://obsidian.md) with the characteristic dotted underline, and here is an [[Internal Link]] as you'd use it in your vault.

---

## Blockquotes

> „Die Grenzen meiner Sprache bedeuten die Grenzen meiner Welt.“
> — Ludwig Wittgenstein

> [!tip] Callout: Tip
> Callouts render with a coloured left border and a serif title. They're great for drawing attention to important notes.

> [!warning] Callout: Warning
> Be careful with this one — the background subtly shifts to signal caution.

> [!info] Callout: Info
> Additional context or background information goes here.

---

## Lists

### Unordered

- Paper texture is generated entirely in CSS
- SVG `feTurbulence` creates the base noise
  - `fractalNoise` for grain and fiber clumps
  - `turbulence` for chaotic blotches
- `feDiffuseLighting` adds 3D surface relief
- Fiber lines run horizontally, vertically, and diagonally

### Ordered

1. Install the theme
2. Open Settings → Appearance
3. Select **Papyrus Nox**
4. Enjoy the aged-paper look

### Checklists

- [x] Dark mode variables
- [x] Paper texture layers
- [x] Heading colours and underlines
- [x] Typography fine-tuning
- [ ] Submit to Community Themes
- [ ] Add screenshots

---

## Tags

#theme #obsidian #dark-mode #papyrus #design #css-only

---

## Code

Inline: The variable `--h1-color: #d4ad6a` defines the gold accent.

```css
/* Letterpress text-shadow on headings */
.markdown-rendered h1 {
  font-family: "Charter", "Iowan Old Style", Georgia, serif;
  color: var(--h1-color);
  text-shadow:
    -1px -1px 3px rgba(0, 0, 0, 0.55),
     1px  1px 2px rgba(255, 255, 255, 0.5);
  border-bottom: 2px dotted var(--h1-color);
}
```

```javascript
// Obsidian plugin example
const plugin = {
  name: "Papyrus Nox",
  version: "1.0.0",
  onload() {
    console.log("Theme loaded ✓");
  }
};
```

---

## Tables

| Feature | Description | Status |
|---|---|---|
| Paper texture | Layered SVG noise + CSS gradients | ✓ Done |
| Heading palette | 6 earthy colours (H1–H6) | ✓ Done |
| Letterpress effect | Dark/light text-shadow | ✓ Done |
| Narrow body text | DM Sans, 14 px, 95 % stretch | ✓ Done |
| Flat sidebar | No texture, #171717 | ✓ Done |
| Light mode | Not supported (dark-only) | — |

---

## Images

Images render with a subtle 92 % opacity that brightens to 100 % on hover, plus rounded corners:

![[example-image.png]]

---

## Horizontal Rules

The lines above and below are `<hr>` elements — they fade in from the edges using a gradient on `--hr-subtle`.

---

## Math (if MathJax/KaTeX is enabled)

Inline math: $E = mc^2$

Display math:

$$
\int_{-\infty}^{\infty} e^{-x^2} \, dx = \sqrt{\pi}
$$

---

## Footnotes

Papyrus Nox uses zero external images[^1] and works offline without any network requests[^2].

[^1]: All textures are generated via inline SVG data URIs and CSS gradients.
[^2]: Fonts fall back to system fonts if DM Sans or Charter aren't installed.

---

## Embedded Content

> [!example] Nested Blockquote with Code
> You can nest elements:
> ```python
> def greet(name: str) -> str:
>     return f"Welcome to Papyrus Nox, {name}!"
> ```
> And continue writing after the code block.

---

## Colour Palette Reference

| Role | Colour | Hex |
|---|---|---|
| **H1 — Gold** | ████ | `#d4ad6a` |
| **H2 — Teal** | ████ | `#78b8a4` |
| **H3 — Mauve** | ████ | `#b48ec0` |
| **H4— Cyan** | ████ | `#7ab8c0` |
| **H5 — Rosé** | ████ | `#c4908e` |
| **H6 — Taupe** | ████ | `#9a9080` |
| Body text | ████ | `#d5d0c8` |
| Muted text | ████ | `#928b82` |
| Background | ████ | `#1e1e1e` |
| Sidebar | ████ | `#171717` |
| Accent | ████ | `#b8976a` |

---

*Papyrus Nox v1.0.0 — MIT License — Björn Kindler*
