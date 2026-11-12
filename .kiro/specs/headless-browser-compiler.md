# Spec: Headless Chromium & Accessibility Tree Compiler (`/.kiro/specs/headless-browser-compiler.md`)

## 1. Objective
Support both lightweight static sites and heavy client-side JavaScript SPAs (React, Next.js, Vue, dynamic e-commerce stores) using a hybrid **Playwright Headless Chromium + Cheerio AST** pipeline.

## 2. Compilation Pipeline
1. **Real Chromium DOM Rendering:**
   - Launches a persistent headless Chromium context via Playwright.
   - Executes client-side JavaScript, waits for network hydration, and captures a visual viewport screenshot (`/screenshots/tab_*.png`) so `Split (Human vs. AI)` mode works even on sites that block `X-Frame-Options` iframes.
2. **98% Bloat Stripping:**
   - Strips scripts, stylesheets, SVGs, tracking pixels, and layout wrappers.
   - Extracts clean paragraphs, pricing tables, clickable navigation links, input boxes, and action buttons.
3. **Safety Brake Classification:**
   - Flags any checkout, purchase, payment, or destructive button before execution.
