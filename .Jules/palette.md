## 2024-02-12 - Missing ARIA label on close buttons
**Learning:** Found multiple instances where the "×" (close) buttons in dialog headers (`dashboard/index.html` and `dashboard/app.js`) were missing `aria-label`s. Because "×" is an icon and read aloud poorly by screen readers, it needs an explicit `aria-label` like "Close dialog" for accessibility.
**Action:** Always verify that buttons with only icons (such as '×', '<svg>') have proper `aria-label` attributes.
