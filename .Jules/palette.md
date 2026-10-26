## 2025-02-19 - Missing ARIA Labels on Icon-only Close Buttons
**Learning:** Text-based icon buttons (like "×" for closing dialogs) are often missed during accessibility audits because they look like text but lack semantic meaning for screen readers. In the dashboard app, `.close-button` elements were missing `aria-label` attributes.
**Action:** Always add `aria-label="Close dialog"` (or similar context-specific labels) to icon-only buttons, even if they use text characters like "×" instead of SVG or font icons.
