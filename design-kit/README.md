# PICO AQSYS — Design Kit

> **One Pico. Many Connected. One AQSYS.**  
> Access · Axis · Intelligence

---

## Overview

This design kit is the single source of truth for the PICO AQSYS front-end visual system. It translates the brand identity into production-ready CSS tokens and components for the AQSYS swarm dashboard and any product surface.

## Files

| File | Purpose |
|---|---|
| `tokens.css` | All design tokens — colors, typography, spacing, radius, shadow, motion, z-index, layout |
| `components.css` | Full component library — buttons, cards, badges, tables, nav, inputs, handoff packets, swarm nodes |
| `index.html` | Living style guide — interactive showcase of every token and component |

## Usage

```html
<!-- In your HTML head -->
<link rel="stylesheet" href="./design-kit/tokens.css" />
<link rel="stylesheet" href="./design-kit/components.css" />
```

Or import in CSS:

```css
@import './design-kit/tokens.css';
@import './design-kit/components.css';
```

## Brand Identity

### Color
| Role | Token | Value |
|---|---|---|
| Primary (Forest Green) | `--color-primary` | `#2B4438` |
| Accent (Gold) | `--color-accent` | `#8B6E2A` |
| Surface Base | `--color-surface-base` | `#F7F5F0` |
| Text Default | `--color-text-default` | `#1A2E24` |

### Typography
- **Display / Headings**: Montserrat — wide tracking, uppercase, geometric
- **Body**: Inter — neutral, readable
- **Code / Data**: JetBrains Mono

### Logo Variants
- **Primary Lockup** — horizontal, mark + wordmark
- **Stacked Lockup** — vertical, mark above wordmark  
- **Icon Mark** — dark green rounded square (app/dashboard)
- **Monogram** — `P →` circled (minimal contexts)

### Brand Symbol Anatomy
| Element | Meaning |
|---|---|
| Central node (PICO) | The trusted local unit of verified action |
| Branching lines (AQSYS) | The intelligent connected colony |
| Arc ring | Access: reach, containment, trusted boundaries |
| Axis arrow | Alignment, coordination, traceability |
| Gold dots | Knowledge flow: continuous learning, evidence |

## Component Reference

### Buttons
```html
<button class="btn btn-primary">Primary</button>
<button class="btn btn-accent">Accent</button>
<button class="btn btn-outline">Outline</button>
<button class="btn btn-ghost">Ghost</button>

<!-- Sizes -->
<button class="btn btn-primary btn-sm">Small</button>
<button class="btn btn-primary btn-lg">Large</button>
```

### Badges
```html
<span class="badge badge-error">Urgent</span>
<span class="badge badge-warning">High</span>
<span class="badge badge-green">Medium</span>
<span class="badge badge-neutral">Low</span>
```

### Cards
```html
<div class="card">...</div>
<div class="card card--tinted">...</div>
<div class="card card--gold">...</div>
```

### Swarm Node
```html
<div class="swarm-node">
  <div class="swarm-node__codename">COMMANDANT</div>
  <div class="swarm-node__name">Regional Command</div>
  <div class="swarm-node__mission">...</div>
</div>
```

### Handoff Packet
```html
<div class="handoff handoff--urgent">
  <div class="handoff__meta">...</div>
  <div class="handoff__summary">...</div>
  <div class="handoff__action">→ Escalate to Commandant</div>
</div>

<!-- Priority modifiers: handoff--urgent | --high | --medium | --low -->
```

### Tables
```html
<div class="table-wrap">
  <table class="table">
    <thead>...</thead>
    <tbody>...</tbody>
  </table>
</div>
```

## Design Principles (from brand)

1. **Evidence first** — surfaces always lead with data, not decoration
2. **Practical clarity** — complexity converted into clear next steps
3. **Field reality** — designed for low-bandwidth, high-stakes environments
4. **Federated** — components are modular and composable across swarms
5. **Warm authority** — the green/gold palette signals trust, not cold tech

## Viewing the Style Guide

Open `index.html` in any browser — no build step required. All fonts load from Google Fonts.

---

*PICO AQSYS · Design Kit v1.0*
