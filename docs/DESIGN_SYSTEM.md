# 🎨 Design System — Moekyawaung Portfolio V3

Complete reference for all design tokens, components, and visual decisions.

---

## Color Palette

### Dark Mode (Default)

| Token | Hex | Role |
|-------|-----|------|
| `--gold` | `#d4a843` | Primary accent, CTA, highlights |
| `--gold-light` | `#f0c96a` | Gradient endpoints, hover states |
| `--gold-dark` | `#a87e28` | Gradient starts, pressed states |
| `--charcoal` | `#1a1a1a` | Page background |
| `--charcoal-2` | `#242424` | Section alternating background |
| `--charcoal-3` | `#2e2e2e` | Card surface, elevated UI |
| `--glass-bg` | `rgba(255,255,255,0.04)` | Glass card fill |
| `--glass-bg2` | `rgba(255,255,255,0.08)` | Glass card hover / input fill |
| `--glass-border` | `rgba(212,168,67,0.18)` | Default card border |
| `--glass-border2` | `rgba(212,168,67,0.35)` | Focused / active border |
| `--text-primary` | `#f5f0e8` | Headings, primary text |
| `--text-muted` | `#a89880` | Body copy, labels |
| `--text-dim` | `#6a5f52` | Placeholders, footer text |

### Light Mode Overrides

| Token | Hex |
|-------|-----|
| `--charcoal` | `#f8f4ee` |
| `--charcoal-2` | `#ede8e0` |
| `--charcoal-3` | `#e0d8cc` |
| `--glass-bg` | `rgba(0,0,0,0.03)` |
| `--glass-bg2` | `rgba(0,0,0,0.06)` |
| `--text-primary` | `#1a1410` |
| `--text-muted` | `#5a4e40` |

---

## Typography

### Font Stack

```css
--font-display: 'Cinzel Decorative', serif;      /* Headings, logo, stats */
--font-body:    'DM Sans', sans-serif;            /* All body text, UI */
--font-mono:    'JetBrains Mono', monospace;      /* Code, labels, chips */
```

### Scale

| Use | Size | Weight | Font |
|-----|------|--------|------|
| Hero name | clamp(2.2rem, 6vw, 4.5rem) | 900 | Display |
| Section title | clamp(1.6rem, 4vw, 2.8rem) | 700 | Display |
| Profile name | 1.1rem | 700 | Display |
| Body large | 1.05rem | 400 | Body |
| Body regular | 1rem | 400 | Body |
| Body small | 0.9rem | 400 | Body |
| Label/chip | 0.72–0.8rem | 500–600 | Mono |
| Section eyebrow | 0.75rem | — | Mono |

---

## Spacing

Compact system — sections use `100px 32px` padding (desktop).

| Breakpoint | Section Padding |
|------------|----------------|
| Desktop (>900px) | `100px 32px` |
| Tablet (600–900px) | `80px 24px` |
| Mobile (<600px) | `70px 20px` |

---

## Border Radius

| Token | Value | Usage |
|-------|-------|-------|
| `--radius-sm` | `8px` | Inputs, small cards, chips |
| `--radius-md` | `16px` | Glass cards, gallery items |
| `--radius-lg` | `24px` | Profile card, newsletter card |
| `--radius-xl` | `40px` | Buttons, pills |

---

## Shadows

| Token | Value | Usage |
|-------|-------|-------|
| `--shadow-gold` | `0 0 40px rgba(212,168,67,0.15)` | Card hover glow |
| `--shadow-card` | `0 8px 40px rgba(0,0,0,0.4)` | Elevated cards |

---

## Glass Card Component

```css
.glass-card {
  background: var(--glass-bg);              /* rgba(255,255,255,0.04) */
  border: 1px solid var(--glass-border);    /* rgba(212,168,67,0.18) */
  border-radius: var(--radius-md);          /* 16px */
  backdrop-filter: blur(20px);
  transition: all 0.3s cubic-bezier(0.4,0,0.2,1);
}
.glass-card:hover {
  border-color: var(--glass-border2);       /* rgba(212,168,67,0.35) */
  box-shadow: var(--shadow-gold);
  transform: translateY(-4px);
}
```

---

## Button Variants

### Primary (Gold Gradient)
```css
background: linear-gradient(135deg, #a87e28, #f0c96a);
color: #1a1a1a;
border-radius: 40px;
padding: 12px 28px;
font-weight: 700;
```

### Outline
```css
background: transparent;
color: #d4a843;
border: 1px solid #d4a843;
border-radius: 40px;
padding: 11px 28px;
```

---

## Animation Easing

```css
--transition: 0.3s cubic-bezier(0.4, 0, 0.2, 1);  /* Default */

/* Reveal animations */
transition: opacity 0.7s ease, transform 0.7s ease;

/* Carousel */
transition: transform 0.5s cubic-bezier(0.4, 0, 0.2, 1);

/* Skill bars */
transition: width 1.4s cubic-bezier(0.4, 0, 0.2, 1);
```

---

## Breakpoints

| Name | Width | Changes |
|------|-------|---------|
| Mobile S | < 500px | Stacked newsletter, single-col footer |
| Mobile M | < 600px | Reduced padding, single-col carousel |
| Tablet | < 768px | 2-col → 1-col grids |
| Tablet L | < 900px | Hero grid stacks, 2-col pricing |
| Desktop | ≥ 900px | Full multi-column layouts |
