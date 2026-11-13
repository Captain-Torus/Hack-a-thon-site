# AgentGate Browser — 2.5-Minute Video Script & Devpost Submission Copy

## Part 1: The 2.5-Minute Demo Video Script

**Before you hit record:**
1. Open `http://localhost:3456` on your **Wikipedia: Spider-Man** tab.
2. Click **`Split (2 AIs Side-by-Side)`** in the top right so both AIs are sitting at the **`0.00s`** starting line.

---

### Scene 1: The Hook & Simultaneous 2-AI Race (0:00 – 0:45)
*(Start on **`Split (2 AIs Side-by-Side)`** with both AIs waiting at `0.00s`)*

> **"Hi judges! Today's AI browser agents have a massive problem: websites were built for human eyes, not AI.**
>
> **Look at the left side of my screen: when a standard AI tries to read a real webpage like Wikipedia's Spider-Man article, it has to wade through tens of thousands of words of raw HTML, CSS, and menus, or take slow screenshots. That wastes time, burns 40 cents a page in tokens, and risks clicking the wrong button.**
>
> **So we built AgentGate Browser—the first headless Chromium web browser that translates the entire web into a 98% smaller, AI-native interface.**
>
> **Watch what happens when we start both AIs at the exact same 0.00-second mark:"**

*(Click the green **`Start Both AIs at 0.00s`** button!)*

> **"Our AgentGate AI on the right strips the page down by over 95% and finishes extracting the key facts and links in 0.42 seconds for 0.04 cents—while the standard AI on the left is still stuck taking screenshots and parsing raw HTML tags!"**

---

### Scene 2: Permanent Default AI & Live AI Browsing (0:45 – 1:30)
*(Click **`AI Browser View`**, then click **`+ New Tab`** at the top left)*

> **"How do you connect your own AI to AgentGate Browser? Instead of copying and pasting text on every single tab, we built a 'Permanent Default AI' bridge.**
>
> **You paste in your AI once right here and click 'Save as Permanent Default AI'. From that moment on, every tab you open automatically syncs to your AI in the background using our Kiro Agent Hooks and `.kiro/live-browser-state.json`."**

*(Click the **`Hacker News Live`** or **`Wikipedia: Spider-Man`** bookmark, and click any link inside the translated page)*

> **"When you browse in AI Browser View, our Playwright Headless Chromium engine loads the real website, strips 100% of the ads and clutter, and gives both you and your AI a clean summary, clickable links that navigate to the next page in AI mode, and an AI Takeout Bag in Simple List, Code Data, or Spreadsheet format."**

---

### Scene 3: The Browser Safety Brake (1:30 – 2:00)
*(Look at the **Action Buttons** table on the right side of the page, and click the red **`Click Button (Triggers Safety Brake)`** next to `Complete Instant Checkout & Pay`)*

> **"What happens if an AI agent tries to click a button that spends money or deletes data? Watch when we click 'Complete Instant Checkout & Pay'—boom!**
>
> **Our Browser Safety Brake immediately freezes the action and pops up this orange Human-in-the-Loop approval bar at the top of the browser. Nothing gets bought or deleted unless the human clicks Approve."**

*(Click **`Block Action`** in the orange bar)*

---

### Scene 4: Kiro Architecture (`/.kiro Specs & Hooks`) (2:00 – 2:25)
*(Click the green **`/.kiro Specs & Hooks`** button in the bookmarks bar)*

> **"Finally, we built AgentGate Browser using Kiro's spec-driven architecture. Right inside the browser, judges can inspect our `.kiro/specs`, steering rules, MCP config, and live Agent Hook execution logs that fire every time a tab navigates or the Safety Brake triggers. Thank you for watching!"**

---

## Part 2: Copy-Paste Answers for the Kiroween Devpost Form

### Project Title
`AgentGate Browser — The AI-Native Headless Web Browser & UI Compiler`

### Tagline (Short Description)
`A headless Chromium web browser that compiles bloated websites into 98% smaller AI-ready pages in milliseconds—with a Permanent Default AI Bridge and a deterministic Safety Brake.`

### Category to Select on Kiroween
- **Primary Category:** `Frankenstein` *(Stitching together two incompatible worlds—bloated human HTML/DOM and fast, deterministic AI agents—into one seamless AI Browser)*
- **Bonus Prizes to Check:** `Best Startup Project ($10,000)` and `Student Prize ($1,500)`

### "How We Used Kiro" (Copy-Paste into the Devpost Kiro Question)
> We used Kiro's spec-driven development workflow (`/.kiro/specs/`), Steering documents (`/.kiro/steering/architecture.md`), Agent Hooks (`/.kiro/hooks/`), and MCP configuration (`/.kiro/mcp/mcp.json`) as the backbone of AgentGate Browser:
> 1. **Kiro Specs (`/.kiro/specs/`):** Before writing the compiler, we defined three modular specifications (`agentgate-translator.md`, `headless-browser-compiler.md`, and `permanent-ai-bridge.md`) to structure how Playwright Chromium HTML is stripped and compiled into 3 Takeout Bag formats (`Simple List`, `Code Data / JSON`, and `Spreadsheet / CSV`) while achieving >90% token compression.
> 2. **Kiro Agent Hooks (`/.kiro/hooks/`):** We implemented two event-driven Kiro hooks (`on-tab-navigate.hook.json` and `on-high-risk-action.hook.json`) that automatically sync all open browser tabs to `.kiro/live-browser-state.json` for the user's Permanent Default AI and freeze checkout/payment actions via our Safety Brake.
> 3. **Kiro Steering (`/.kiro/steering/architecture.md`):** Enforced strict plain-English UI rules, high-contrast developer aesthetics, and zero-trust financial action interception across every component.
