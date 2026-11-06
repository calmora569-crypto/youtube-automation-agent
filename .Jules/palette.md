## 2025-02-19 - Missing ARIA Labels on Icon-only Close Buttons
**Learning:** Text-based icon buttons (like "×" for closing dialogs) are often missed during accessibility audits because they look like text but lack semantic meaning for screen readers. In the dashboard app, `.close-button` elements were missing `aria-label` attributes.
**Action:** Always add `aria-label="Close dialog"` (or similar context-specific labels) to icon-only buttons, even if they use text characters like "×" instead of SVG or font icons.
## 2025-02-19 - Loading states for async form submissions
**Learning:** Adding immediate visual feedback (like "Saving...", "Starting...") and disabling the submit button during async form submissions prevents duplicate clicks and makes the UI feel much more responsive and trustworthy.
**Action:** When adding submit event listeners for forms that trigger async API calls, always store the submitter button's text, disable it, update text to a loading state, and restore it in a `finally` block or after the promise resolves.
