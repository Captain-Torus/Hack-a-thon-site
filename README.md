# AgentGate Browser — The AI-Native Headless Web Browser & UI Compiler

**AgentGate Browser** is a headless Chromium AI web browser that translates bloated human websites (100,000+ words of HTML, CSS, trackers, and layout divs) into a **98% smaller, structured AI-friendly interface** in milliseconds—complete with a **Permanent Default AI Bridge** and a deterministic **Safety Brake** for financial/destructive actions.

---

## Why We Built AgentGate Browser

Today's AI browser agents are broken in three ways:
1. **Slow & Expensive:** Sending full-page screenshots or 100,000 words of raw DOM to a vision/language model takes **30–45 seconds per click** and costs **$0.40+ per page**.
2. **Constant Re-Pasting:** Users have to manually copy and paste page text into their AI on every single tab.
3. **Unsafe Autonomous Clicks:** Giving an AI agent raw access to click buttons on a page risks accidental purchases, subscriptions, or deleted data.

**AgentGate Browser solves all three:**
- **Headless Chromium Compiler (`98% Smaller`):** Renders modern JavaScript websites via Playwright Chromium and compiles them into a clean **AI Takeout Bag** (*Simple List*, *Code Data / JSON*, or *Spreadsheet / CSV*) in `<200ms`.
- **Permanent Default AI Bridge:** Paste your AI once and save it as your **Permanent Default AI**. Every tab you open, search you run, or link you click is automatically synced to `.kiro/live-browser-state.json` and `/api/permanent-ai/feed`—your AI always has live access to all your open tabs without copy-pasting.
- **Deterministic Safety Brake:** Automatically intercepts any button containing payment, checkout, purchase, or delete actions, freezing execution and displaying an approval banner for the human user.
- **3 Built-in View Modes:**
  1. `AI Browser View` — Browse the web in clean, ad-free AI mode where clicking any link navigates to and translates the next page.
  2. `Split (Human vs AI)` — Side-by-side comparison of the real Headless Chromium visual screenshot vs. the condensed AI translation.
  3. `Hackathon Race Demo` — Live benchmark comparing a standard screenshot-based browser agent (`34.2s`, `$0.42`) against AgentGate Browser (`<0.2s`, `$0.0004`).

---

## Built with Kiro (`/.kiro` Architecture)

This repository includes our full Kiro spec-driven development suite in [`/.kiro/`](./.kiro):
- **Specs ([`/.kiro/specs/`](./.kiro/specs)):**
  - [`agentgate-translator.md`](./.kiro/specs/agentgate-translator.md) — Core DOM-to-Takeout-Bag compilation & Safety Brake specification
  - [`permanent-ai-bridge.md`](./.kiro/specs/permanent-ai-bridge.md) — Permanent Default AI auto-sync specification
  - [`headless-browser-compiler.md`](./.kiro/specs/headless-browser-compiler.md) — Playwright Headless Chromium & Split-View rendering spec
- **Steering ([`/.kiro/steering/architecture.md`](./.kiro/steering/architecture.md)):** Enforces plain-English UX, Obsidian & Emerald developer aesthetics, and zero-trust Safety Brake rules.
- **Agent Hooks ([`/.kiro/hooks/`](./.kiro/hooks)):**
  - [`on-tab-navigate.hook.json`](./.kiro/hooks/on-tab-navigate.hook.json) — Automatically syncs all open browser tabs to the user's Permanent Default AI on every navigation event.
  - [`on-high-risk-action.hook.json`](./.kiro/hooks/on-high-risk-action.hook.json) — Halts execution and triggers human-in-the-loop verification whenever a financial or destructive action is clicked.
- **MCP Configuration ([`/.kiro/mcp/mcp.json`](./.kiro/mcp/mcp.json)):** Connects external agents directly to the live AgentGate Browser state.

---

## Quick Start (Run Locally in 30 Seconds)

```bash
git clone https://github.com/YOUR_USERNAME/agentgate-browser.git
cd agentgate-browser
npm install
npx playwright install chromium
npm start
```

Then open **`http://localhost:3456`** in your browser.

---

## License

MIT License — see [LICENSE](./LICENSE).
