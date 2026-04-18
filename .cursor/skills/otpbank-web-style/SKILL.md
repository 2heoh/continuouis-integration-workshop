---
name: otpbank-web-style
description: Create marketing and product web pages in a clean, bank-grade visual style similar to otpbank.ru (white background, generous spacing, strong typography, subtle borders/shadows, rounded cards, calm accent color). Use when the user asks to "make it look like otpbank.ru", "OTP Bank style", "bank website style", or wants a modern, trustworthy corporate landing page UI.
---

# OTP Bank–like Web Style

## Goal

Produce web pages with a **calm, trustworthy, corporate banking** look:
- lots of white space, clear hierarchy
- large headings, readable body text
- rounded cards, light dividers, minimal shadows
- restrained accent color and minimal visual noise

Important: **do not copy** OTP Bank assets (logos, illustrations, text, exact layout). Recreate the *style and UX patterns*.

## Default design tokens (adjust per project)

- **Layout**
  - Max content width: 1200–1240px
  - Gutters: 16px (mobile), 24px (tablet), 32px (desktop)
  - Section padding: 56–96px vertical (desktop), 32–56px (mobile)
  - Corner radius: 12–16px (cards, inputs, buttons)

- **Typography**
  - Use a modern sans (system font stack by default).
  - H1: 40–56px, 1.05–1.15 line-height
  - H2: 28–36px, 1.15–1.25
  - Body: 16–18px, 1.5–1.7
  - Subtle secondary text: muted gray, not smaller than 14px

- **Color**
  - Background: #FFFFFF
  - Surface: #F6F7F9 (optional for sections)
  - Text: near-black (#111–#1A)
  - Muted text: #5B6472 (approx.)
  - Border: #E6E8EE (approx.)
  - Accent: pick **one** brand-like color and use it consistently for CTAs/links

- **Elevation**
  - Prefer borders over shadows.
  - If a shadow is used: very soft, low opacity, small blur.

## Page structure blueprint

Use this order unless user asks otherwise:

1. **Header**
   - Left: logo/name
   - Center or right: primary nav (3–6 items)
   - Right: primary CTA (e.g., “Оформить”, “Войти”)

2. **Hero**
   - Large H1 + short supporting text
   - Primary CTA + secondary CTA (outline or link)
   - Optional: product visual (illustration or simple device mock)

3. **Trust / benefits**
   - 3–6 benefit cards with icons
   - Short, scannable copy

4. **Product blocks**
   - Alternating image/text sections
   - Clear feature bullets

5. **Rates / pricing / conditions** (if relevant)
   - Table or card grid
   - Footnotes and disclaimers clearly separated and readable

6. **FAQ**
   - Accordion with 6–10 questions

7. **Footer**
   - Columns: products, company, help
   - Legal/disclaimer area

## Component patterns

- **Buttons**
  - Primary: filled accent, bold label, 44–48px height
  - Secondary: outline or soft surface
  - Keep states: hover/focus/disabled clearly visible

- **Cards**
  - Rounded, border, soft background
  - Title + 1–3 lines description + optional link

- **Forms**
  - Labels above inputs
  - Helper/error text below
  - Inputs 44–48px height, large click targets

- **Navigation**
  - Clear active state
  - Sticky header optional for long pages

## Accessibility and quality bar

- Keyboard navigation works (focus styles visible).
- Contrast is sufficient for text on white/surface backgrounds.
- Tap targets >= 44px.
- Responsive layout for 360px width without horizontal scroll.

## Workflow (how to apply this style)

1. Identify page purpose (landing / product / help) and primary CTA.
2. Draft content hierarchy: hero → benefits → details → FAQ.
3. Build layout with a strict grid and consistent spacing scale.
4. Apply restrained palette: one accent, soft neutrals, minimal gradients.
5. Validate: scanability (headings), trust cues (clarity, disclaimers), mobile.

## Output expectations

When generating a page:
- Provide **HTML + CSS** (or React) with a small set of reusable classes/components.
- Use a consistent spacing scale (e.g., 8px base).
- Include at least: header, hero, benefit cards, FAQ, footer.
