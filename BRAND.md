<p align="center">
  <img src="assets/banner.svg" alt="dirtysouthalpha — AURORA-X neon brand kit">
</p>

# AURORA-X neon — brand kit

The shared visual identity for every dirtysouthalpha repo. The goal is a family that
reads as **one product line**: flashy but clean, never crowded. **One** strong element
of each kind per repo, generous whitespace. A wall of badges or competing animations is
a failure — restraint is the point.

## Palette (locked)

| Role | Hex | Use |
| --- | --- | --- |
| Canvas | `#0A0A0F` | near-black background, everywhere |
| Primary | `#22D3EE` | electric cyan — wordmark glow, main accent |
| Secondary | `#8B5CF6` | violet — accent line, gradient partner |
| Text | `#E8E8F0` | off-white body / wordmark highlight |
| Muted | `#6B7280` | slate — taglines, secondary labels |

**Motion:** one slow cyan → violet gradient sweep, ≤ 4s loop, subtle. Never more than one
moving thing on a page.

## Type

Geometric / monospace wordmark — **JetBrains Mono** (or a Space Grotesk vibe). Heavy weight,
slight letter-spacing. Body copy stays in the reader's default. No copyrighted font files —
JetBrains Mono is SIL OFL; web-safe mono stacks are the fallback in SVG.

## Banner template

Every repo's `assets/banner.svg` is the same hand-authored animated SVG:

- Deep `#0A0A0F` canvas, faint dot texture, a prompt-glyph motif box.
- **Repo name as the wordmark** in the cyan → violet gradient, with the slow sheen sweep.
- **One** muted tagline line, then a single thin cyan → violet accent rule.
- Vary only the name, the tagline, and the one motif glyph. Nothing else moves.

Put it at the very top of the README:

```html
<p align="center"><img src="assets/banner.svg" alt="<repo> — <tagline>"></p>
```

## Badges

One centered row, **4–6 max**: license, version/release, primary language, one "built with".
Palette-colored, flat:

```
https://img.shields.io/badge/<label>-<msg>-22D3EE?style=flat-square&labelColor=0A0A0F
```

Use violet (`8B5CF6`) for the single "built with" badge; cyan for the rest. No badge walls,
no stat-card spam, no visitor counters, no emoji soup.

## Terminal demos (CLI / agent repos only)

One styled dark terminal cast (`assets/demo.svg`) after the banner, showing a **real or
honestly-representative** command — `--help`, a dry-run, or actual tool output. Never fake
success text.

## Social preview

`1280×640` `.github/social-preview.png` in the same style (gradient wordmark + tagline +
accent rule). GitHub's social-preview upload is web-only — set it under
*Settings → General → Social preview*.

## How to reuse

New repo or plugin? Copy `assets/banner.svg`, change the wordmark + tagline + one glyph,
keep every hex above exactly. That's the whole system — stay on it and the family stays tight.
