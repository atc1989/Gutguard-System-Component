---
title: GutGuard Portable CSS Starter
tags: [gutguard, css, implementation, design-system]
updated: 2026-08-13
---

# Portable CSS starter

This stylesheet carries the system's visual tokens and common component skins without copying any page layout. Rename the `gg-` classes to match the destination system.

```css
:root {
  color-scheme: light;

  --gg-bone: #f4f1ea;
  --gg-bone-soft: #ebe7de;
  --gg-bone-deep: #ddd7c8;
  --gg-paper: #fcfaf5;

  --gg-blue: #0608a9;
  --gg-blue-press: #04067a;
  --gg-gold: #b08d5b;
  --gg-gold-soft: #c9ac7e;

  --gg-ink: #0f0f18;
  --gg-ink-2: #3a3a48;
  --gg-ink-3: #6b6b7a;
  --gg-ink-4: #a0a0ae;
  --gg-rule: #d8d2c2;
  --gg-rule-soft: #e5e0d2;
  --gg-error: #b0202e;

  --gg-serif: "Fraunces", "Times New Roman", serif;
  --gg-sans: "Inter Tight", system-ui, -apple-system, "Segoe UI", sans-serif;
  --gg-mono: ui-monospace, SFMono-Regular, Menlo, Consolas, monospace;

  --gg-r-sm: 10px;
  --gg-r-md: 14px;
  --gg-r-lg: 24px;
  --gg-r-pill: 999px;

  --gg-shadow-card: 0 14px 36px rgba(15, 15, 24, 0.07);
  --gg-shadow-modal: 0 24px 80px rgba(15, 15, 24, 0.28);
  --gg-ease-out: cubic-bezier(0.22, 1, 0.36, 1);
}

/* Visual foundation only; attach this class to the destination surface. */
.gg-surface {
  color: var(--gg-ink);
  background-color: var(--gg-bone);
  background-image: radial-gradient(
    circle at 1px 1px,
    rgba(15, 15, 24, 0.025) 1px,
    transparent 0
  );
  background-size: 3px 3px;
  font-family: var(--gg-sans);
  font-size: 16px;
  line-height: 1.5;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

.gg-display {
  margin: 0;
  color: var(--gg-ink);
  font-family: var(--gg-serif);
  font-size: clamp(46px, 7vw, 72px);
  font-weight: 400;
  letter-spacing: -0.025em;
  line-height: 0.95;
  text-wrap: balance;
}

.gg-display em {
  color: var(--gg-blue);
  font-style: italic;
  font-weight: 400;
}

.gg-heading {
  margin: 0;
  color: var(--gg-ink);
  font-family: var(--gg-serif);
  font-size: clamp(28px, 4vw, 46px);
  font-weight: 400;
  line-height: 1.04;
}

.gg-lede {
  color: var(--gg-ink-2);
  font-family: var(--gg-serif);
  font-size: 18px;
  line-height: 1.42;
}

.gg-eyebrow {
  color: var(--gg-blue);
  font-size: 10px;
  font-weight: 900;
  letter-spacing: 0.16em;
  text-transform: uppercase;
}

.gg-help {
  color: var(--gg-ink-3);
  font-size: 12px;
  line-height: 1.45;
}

.gg-card {
  border: 1px solid var(--gg-rule);
  border-radius: var(--gg-r-md);
  background: var(--gg-paper);
  padding: clamp(16px, 2.4vw, 24px);
  box-shadow: var(--gg-shadow-card);
}

.gg-card--editorial {
  border-radius: 0;
  background: var(--gg-bone);
  box-shadow: none;
}

.gg-button {
  min-height: 48px;
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: 10px;
  border: 0;
  border-radius: var(--gg-r-sm);
  padding: 12px 18px;
  font: inherit;
  font-weight: 800;
  cursor: pointer;
  transition: background-color 0.2s ease, color 0.2s ease,
    border-color 0.2s ease, transform 0.1s ease;
}

.gg-button--primary {
  background: var(--gg-blue);
  color: var(--gg-bone);
}

.gg-button--primary:hover:not(:disabled) {
  background: var(--gg-blue-press);
}

.gg-button--editorial {
  min-height: 62px;
  justify-content: space-between;
  border-radius: 0;
  background: var(--gg-ink);
  color: var(--gg-bone);
  padding: 18px 24px;
}

.gg-button--editorial:hover:not(:disabled) {
  background: var(--gg-blue);
}

.gg-button--secondary {
  border: 1px solid var(--gg-rule);
  background: rgba(252, 250, 245, 0.72);
  color: var(--gg-ink);
  font-size: 12px;
  font-weight: 900;
  letter-spacing: 0.08em;
  text-transform: uppercase;
}

.gg-button--secondary:hover:not(:disabled) {
  border-color: var(--gg-blue);
  color: var(--gg-blue);
}

.gg-button:active:not(:disabled) {
  transform: scale(0.99);
}

.gg-button:disabled {
  background: var(--gg-bone-soft);
  color: var(--gg-ink-4);
  cursor: not-allowed;
}

.gg-button:focus-visible,
.gg-link:focus-visible {
  outline: 3px solid var(--gg-gold);
  outline-offset: 3px;
}

.gg-field {
  display: grid;
  gap: 7px;
}

.gg-field__label {
  color: var(--gg-ink-3);
  font-size: 10px;
  font-weight: 900;
  letter-spacing: 0.14em;
  text-transform: uppercase;
}

.gg-field__control {
  width: 100%;
  min-height: 48px;
  border: 1px solid var(--gg-rule);
  border-radius: var(--gg-r-sm);
  background: var(--gg-bone);
  padding: 12px 14px;
  color: var(--gg-ink);
  font: inherit;
  outline: none;
}

.gg-field__control::placeholder {
  color: var(--gg-ink-4);
}

.gg-field__control:hover {
  border-color: var(--gg-ink-4);
}

.gg-field__control:focus-visible {
  border-color: var(--gg-blue);
  box-shadow: 0 0 0 3px rgba(6, 8, 169, 0.14);
}

.gg-field__control[aria-invalid="true"] {
  border-color: var(--gg-error);
}

.gg-field__error {
  color: var(--gg-error);
  font-size: 12px;
  font-weight: 800;
}

.gg-segment {
  display: inline-grid;
  grid-auto-flow: column;
  gap: 4px;
  border: 1px solid var(--gg-rule);
  border-radius: var(--gg-r-md);
  background: var(--gg-bone-soft);
  padding: 4px;
}

.gg-segment__button {
  min-height: 44px;
  border: 0;
  border-radius: var(--gg-r-sm);
  background: transparent;
  padding: 8px 14px;
  color: var(--gg-ink-3);
  font: inherit;
  font-size: 12px;
  font-weight: 800;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  cursor: pointer;
}

.gg-segment__button[aria-selected="true"],
.gg-segment__button.is-active {
  background: var(--gg-paper);
  color: var(--gg-ink);
  box-shadow: 0 2px 7px rgba(15, 15, 24, 0.09);
}

.gg-badge {
  display: inline-flex;
  align-items: center;
  border: 1px solid var(--gg-rule);
  border-radius: var(--gg-r-pill);
  padding: 4px 10px;
  color: var(--gg-ink-3);
  font-size: 10px;
  font-weight: 900;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  white-space: nowrap;
}

.gg-badge--active {
  border-color: rgba(6, 8, 169, 0.32);
  color: var(--gg-blue);
}

.gg-alert {
  border: 1px solid var(--gg-rule);
  border-radius: var(--gg-r-md);
  background: rgba(235, 231, 222, 0.66);
  padding: 13px 15px;
  color: var(--gg-blue);
  font-weight: 700;
}

.gg-alert--error {
  border-color: rgba(176, 32, 46, 0.32);
  background: rgba(176, 32, 46, 0.07);
  color: #8f1824;
}

.gg-backdrop {
  background: rgba(15, 15, 24, 0.58);
  backdrop-filter: blur(3px);
}

/* —— File attachment (never show native file chrome) —— */
.gg-file {
  position: relative;
}

.gg-file__input {
  position: absolute;
  width: 1px;
  height: 1px;
  padding: 0;
  margin: -1px;
  overflow: hidden;
  clip: rect(0, 0, 0, 0);
  white-space: nowrap;
  border: 0;
}

.gg-file__zone {
  display: block;
  border: 1.5px dashed var(--gg-rule);
  border-radius: var(--gg-r-md);
  background: var(--gg-bone);
  padding: 22px 18px;
  text-align: center;
  cursor: pointer;
  color: var(--gg-ink);
}

.gg-file__zone:hover,
.gg-file:focus-within .gg-file__zone {
  border-color: var(--gg-blue);
  background: rgba(6, 8, 169, 0.04);
}

.gg-file__zone.is-error {
  border-color: var(--gg-error);
  background: rgba(176, 32, 46, 0.05);
}

.gg-file__icon {
  display: inline-grid;
  place-items: center;
  width: 44px;
  height: 44px;
  margin: 0 auto 10px;
  border: 1px solid var(--gg-rule);
  border-radius: var(--gg-r-sm);
  background: var(--gg-paper);
  color: var(--gg-ink-3);
}

.gg-file__zone:hover .gg-file__icon {
  color: var(--gg-blue);
  border-color: var(--gg-blue);
}

.gg-file__title {
  display: block;
  margin-bottom: 4px;
  font-size: 15px;
  font-weight: 700;
}

.gg-file__hint {
  display: block;
  margin-bottom: 14px;
  color: var(--gg-ink-3);
  font-size: 13px;
}

.gg-file__zone.is-error .gg-file__hint {
  color: #8f1824;
}

.gg-file__row {
  display: flex;
  align-items: center;
  gap: 12px;
  padding: 12px 14px;
  border: 1px solid var(--gg-rule);
  border-radius: var(--gg-r-sm);
  background: var(--gg-paper);
}

.gg-file__row.is-error {
  border-color: var(--gg-error);
}

.gg-file__type {
  width: 36px;
  height: 36px;
  display: grid;
  place-items: center;
  flex-shrink: 0;
  border-radius: 8px;
  background: rgba(6, 8, 169, 0.08);
  color: var(--gg-blue);
  font-size: 11px;
  font-weight: 800;
}

.gg-file__name {
  font-size: 14px;
  font-weight: 700;
}

.gg-file__meta {
  font-size: 12px;
  color: var(--gg-ink-3);
}

.gg-file__progress {
  height: 6px;
  margin-top: 10px;
  border-radius: var(--gg-r-pill);
  background: var(--gg-bone-soft);
  overflow: hidden;
}

.gg-file__progress > i {
  display: block;
  height: 100%;
  background: var(--gg-blue);
  border-radius: inherit;
}

/* —— Icon button (Lucide-style SVG, currentColor) —— */
.gg-icon-btn {
  width: 44px;
  height: 44px;
  display: inline-grid;
  place-items: center;
  border: 1px solid var(--gg-rule);
  border-radius: var(--gg-r-sm);
  background: var(--gg-paper);
  color: var(--gg-ink);
  cursor: pointer;
  flex-shrink: 0;
}

.gg-icon-btn svg {
  width: 20px;
  height: 20px;
  stroke: currentColor;
  fill: none;
  stroke-width: 2;
  stroke-linecap: round;
  stroke-linejoin: round;
}

.gg-icon-btn:hover:not(:disabled) {
  border-color: var(--gg-blue);
  color: var(--gg-blue);
}

.gg-icon-btn:disabled {
  color: var(--gg-ink-4);
  cursor: not-allowed;
}

.gg-icon-btn--dense {
  width: 36px;
  height: 36px;
}

.gg-icon-btn--ghost {
  border-color: transparent;
  background: transparent;
}

.gg-icon-btn--square {
  border-radius: 0;
}

/* —— Dialog (structured header / body / footer) —— */
.gg-dialog {
  display: flex;
  flex-direction: column;
  width: min(100%, 520px);
  border: 1px solid var(--gg-rule);
  border-radius: var(--gg-r-lg);
  background: var(--gg-paper);
  box-shadow: var(--gg-shadow-modal);
  overflow: hidden;
}

.gg-dialog--square {
  border-radius: 0;
}

.gg-dialog-header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 12px;
  padding: 18px 20px;
  border-bottom: 1px solid var(--gg-rule);
}

.gg-dialog-header h2,
.gg-dialog-title {
  margin: 0;
  font-family: var(--gg-serif);
  font-size: 28px;
  font-weight: 400;
  line-height: 1.1;
  letter-spacing: -0.02em;
  color: var(--gg-ink);
}

.gg-dialog-body {
  padding: 20px;
  color: var(--gg-ink-2);
  font-size: 14px;
  line-height: 1.5;
  overflow: auto;
  max-height: min(50vh, 360px);
}

.gg-dialog-footer {
  display: flex;
  justify-content: flex-end;
  gap: 10px;
  padding: 16px 20px;
  border-top: 1px solid var(--gg-rule);
}

/* —— Switch —— */
.gg-switch {
  position: relative;
  width: 44px;
  height: 26px;
  border: 0;
  border-radius: var(--gg-r-pill);
  background: var(--gg-bone-deep);
  cursor: pointer;
  flex-shrink: 0;
  transition: background 0.18s var(--gg-ease-out);
}

.gg-switch::after {
  content: "";
  position: absolute;
  top: 3px;
  left: 3px;
  width: 20px;
  height: 20px;
  border-radius: 50%;
  background: var(--gg-paper);
  box-shadow: 0 1px 3px rgba(15, 15, 24, 0.18);
  transition: transform 0.18s var(--gg-ease-out);
}

.gg-switch[aria-checked="true"] {
  background: var(--gg-blue);
}

.gg-switch[aria-checked="true"]::after {
  transform: translateX(18px);
}

.gg-switch-row {
  display: inline-flex;
  align-items: center;
  gap: 12px;
  font-size: 14px;
  font-weight: 600;
  color: var(--gg-ink);
}

/* —— Accordion chevron (pair with .gg-icon-btn--ghost) —— */
.gg-acc-head {
  width: 100%;
  min-height: 52px;
  padding: 12px 16px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 12px;
  font-weight: 700;
  text-align: left;
  background: transparent;
  border: 0;
  cursor: pointer;
  color: inherit;
}

.gg-acc-head .gg-chev {
  color: var(--gg-ink-3);
  transition: transform 0.2s var(--gg-ease-out), color 0.2s var(--gg-ease-out);
}

.gg-acc-item[data-open="true"] .gg-acc-head .gg-chev,
.gg-acc-item.open .gg-acc-head .gg-chev {
  transform: rotate(180deg);
  color: var(--gg-blue);
}

@media (prefers-reduced-motion: reduce) {
  .gg-button,
  .gg-segment__button,
  .gg-switch,
  .gg-switch::after,
  .gg-acc-head .gg-chev {
    scroll-behavior: auto;
    transition-duration: 0.01ms;
  }
}
```


## Optional editorial ruled field

Use this variant for the square registration dialect instead of the boxed field.

```css
.gg-ruled-field {
  border-bottom: 1px solid var(--gg-rule);
  padding: 18px 0;
}

.gg-ruled-field:focus-within {
  border-bottom-color: var(--gg-blue);
}

.gg-ruled-field__label {
  color: var(--gg-ink-3);
  font-family: var(--gg-serif);
  font-size: 14px;
  font-style: italic;
}

.gg-ruled-field__control {
  border: 0;
  border-radius: 0;
  background: transparent;
  padding: 4px 0;
  color: var(--gg-ink);
  font: 500 17px/1.4 var(--gg-sans);
  outline: 0;
}

.gg-ruled-field:focus-within .gg-ruled-field__label {
  color: var(--gg-blue);
}

.gg-ruled-field.has-error {
  border-bottom-color: var(--gg-error);
}

.gg-ruled-field.has-error .gg-ruled-field__label {
  color: var(--gg-error);
}
```

## Variables supplied beyond the original stylesheet

The source CSS references several undefined names. For portability, map them as follows:

| Original reference | Safe portable value |
|---|---|
| `--paper` | `#FCFAF5` |
| `--cream` | `#FCFAF5` or `#F4F1EA` |
| `--rule-strong` | `#C8C0AE` |
| `--mono` | `ui-monospace, SFMono-Regular, Menlo, Consolas, monospace` |
| `--heat` | `#B5431F` |
| `--recovery` | `#1E6FB8` |

## Usage rule

Choose either the rounded component classes or the editorial square modifiers for a given product surface. Keep the tokens identical so separate systems still read as the same GutGuard brand.

