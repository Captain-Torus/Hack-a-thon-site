# AgentGate Browser — 2.5-Minute Video Script & Devpost Submission Copy

## Part 1: The 2.5-Minute Demo Video Script

**Before you hit record:**
1. Open `http://localhost:3456` on the **`Pricing & Fees` (`stripe.com/pricing`)** tab.
2. Click **`Split (2 AIs Side-by-Side)`** in the top right so both AIs are sitting at the **`0.00s`** starting line.

---

### Part 1: The Problem & 2-AI Race (0:00 – 0:45)
*(Keep your screen on **`Split (2 AIs Side-by-Side)`** on the Stripe Pricing tab)*

**"Hi judges! Today's AI browser agents have a big problem: websites were built for human eyes, not AI."**

**"Whether your AI is trying to book a flight, compare prices across online stores, or read a company webpage like Stripe on the left, a normal AI has to dig through over 240,000 words of messy HTML, CSS, and ads, or take slow screenshots. That takes 35 seconds a click, costs 40 cents a page, and can accidentally click the wrong button."**

**"So we built AgentGate Browser—a universal headless Chromium web browser that can translate almost any website on the internet into a 99% smaller, AI-ready page in milliseconds."**

**"Watch what happens when we start both AIs at the exact same 0.00-second mark:"**

👉 **[CLICK: the green `Start Both AIs at 0.00s` button]**

**"Our AgentGate AI on the right shrinks Stripe's 244,000-word page down to 656 clean words—99.7% smaller—and finishes in 0.42 seconds for a fraction of a cent, while the normal AI on the left is still stuck taking screenshots and reading raw code!"**

---

### Part 2: Real-World Use Cases & Permanent Default AI (0:45 – 1:35)
👉 **[CLICK: `AI Browser View` in the top right, then click `+ New Tab` in the top left]**

**"Because AgentGate works across the entire web, you can use it for real-world jobs like searching and booking flights, comparing products across multiple tabs, or pulling live research into docs."**

**"And instead of copying and pasting text on every single tab, we built a 'Permanent Default AI' option. You paste in your AI once right here and click 'Save as Permanent Default AI'. From that moment on, every tab you open automatically syncs to your AI in the background using our Kiro Agent Hooks."**

👉 **[CLICK: the `Kiroween Hackathon Page (-99.1%)` bookmark]**

**"Look how fast it translates the live Kiroween Hackathon page itself! Our Headless Chromium engine loads any real website, removes 100% of the clutter, and gives you and your AI a clean summary, clickable links that translate the next page, and an AI Takeout Bag in Simple List, Code Data, or Spreadsheet format."**

---

### Part 3: The Browser Safety Brake (Safe Flight & Shopping Checkout) (1:35 – 2:05)
👉 **[CLICK: the red `Click Button (Triggers Safety Brake)` button in the Action Buttons table on the right]**

**"Now imagine your AI found the right flight or product and tries to click a button that spends money or deletes data. Watch when we click 'Complete Instant Checkout & Pay'—boom!"**

**"Our Browser Safety Brake immediately freezes the click and pops up this orange approval bar at the top of the screen. Your AI can do 99% of the legwork, while nothing gets bought or deleted unless the human clicks Approve."**

👉 **[CLICK: `Block Action` in the orange bar]**

---

### Part 4: Kiro Specs & Hooks (2:05 – 2:30)
👉 **[CLICK: the green `/.kiro Specs & Hooks` button in the bookmarks bar]**

**"Finally, we built AgentGate Browser using Kiro's spec-driven architecture. Right inside the browser, judges can inspect our `.kiro/specs`, steering rules, MCP config, and live Agent Hook logs that fire every time a tab navigates or the Safety Brake triggers. Thank you for watching!"**

---

## Part 2: Copy-Paste Answers for the Kiroween Devpost Form

### Project Title
`AgentGate Browser — The AI-Native Headless Web Browser & UI Compiler`

### Tagline (Short Description)
`A universal headless Chromium web browser that compiles bloated websites into 99% smaller AI-ready pages in milliseconds—with a Permanent Default AI Bridge and a deterministic Safety Brake.`

### Category to Select on Kiroween
- **Primary Category:** `Frankenstein` *(Stitching together two incompatible worlds—bloated human HTML/DOM and fast, deterministic AI agents—into one seamless AI Browser)*
- **Bonus Prizes to Check:** `Best Startup Project ($10,000)` and `Student Prize ($1,500)`

### "How We Used Kiro" (Copy-Paste into the Devpost Kiro Question)
> We used Kiro's spec-driven development workflow (`/.kiro/specs/`), Steering documents (`/.kiro/steering/architecture.md`), Agent Hooks (`/.kiro/hooks/`), and MCP configuration (`/.kiro/mcp/mcp.json`) as the backbone of AgentGate Browser:
> 1. **Kiro Specs (`/.kiro/specs/`):** Before writing the compiler, we defined three modular specifications (`agentgate-translator.md`, `headless-browser-compiler.md`, and `permanent-ai-bridge.md`) to structure how Playwright Chromium HTML is stripped and compiled into 3 Takeout Bag formats (`Simple List`, `Code Data / JSON`, and `Spreadsheet / CSV`) while achieving >99% token compression on complex websites.
> 2. **Kiro Agent Hooks (`/.kiro/hooks/`):** We implemented two event-driven Kiro hooks (`on-tab-navigate.hook.json` and `on-high-risk-action.hook.json`) that automatically sync all open browser tabs to `.kiro/live-browser-state.json` for the user's Permanent Default AI and freeze checkout/payment actions via our Safety Brake.
> 3. **Kiro Steering (`/.kiro/steering/architecture.md`):** Enforced strict plain-English UI rules, high-contrast developer aesthetics, and zero-trust financial action interception across every component.
