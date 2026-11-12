# AgentGate Browser — 3-Minute Video Script & Devpost Submission Copy

## Part 1: The 3-Minute Demo Video Script (Record with QuickTime or Loom)

**Total Time:** ~2 minutes 35 seconds (Judges love videos under 2:45 that jump straight into the live demo!)

---

### [0:00 – 0:25] The Hook & Problem (Show `Split (Human vs AI)` View on Screen)
> **"Hi judges! Today's AI browser agents have a massive problem: websites were built for human eyes, not AI. When an AI tries to browse a normal site, it's forced to read 50,000 to 100,000 words of bloated HTML, CSS, and ads—or take slow screenshots. That takes 35 seconds per click, costs 40 cents a page, and worse—if the AI clicks the wrong button, it can accidentally buy something or delete your data.**
>
> **So we built AgentGate Browser: the first headless Chromium web browser that translates the entire web into a 98% smaller, AI-native interface in milliseconds."**

---

### [0:25 – 1:10] Live Demo 1: Browsing + Permanent Default AI (Switch to `AI Browser View`)
*(Click `+ New Tab` to show the clean New Tab screen and the **Permanent Default AI** box)*
> **"First, instead of copying and pasting text on every single tab, AgentGate has a 'Permanent Default AI' bridge. You paste in your AI once—and click 'Save as Permanent Default AI'. From that moment on, every tab you open is automatically synced to your AI via our Kiro Agent Hooks and `.kiro/live-browser-state.json`."**
>
> *(Click a Quick Bookmark like `Book Store` or type `qbreader.org`, then click a link inside the translated page)*
> **"Watch how fast this is: our Playwright Headless Chromium engine renders the real website, strips 100% of the ads and layout clutter, and gives both you and your AI a clean summary, clickable sub-page links, and a formatted AI Takeout Bag in Simple List, JSON, or CSV. When I just opened QBReader in a tab, my Permanent AI automatically read my live tab, navigated into the database, and calculated that 10.8% of all History questions are about France—without me copying or pasting a single word."**

---

### [1:10 – 1:45] Live Demo 2: The Browser Safety Brake
*(Scroll to the Action Buttons table on any tab and click the red `Complete Instant Checkout & Pay` button)*
> **"Second, what happens if your AI tries to click a button that spends money or deletes data? Watch when we click 'Complete Instant Checkout & Pay'—boom! Our Browser Safety Brake immediately freezes the action and pops up this orange Human-in-the-Loop approval banner at the top of the browser. Nothing gets purchased unless the human clicks Approve."**

---

### [1:45 – 2:15] Live Demo 3: Hackathon Speed & Cost Race (`Hackathon Race Demo` Tab)
*(Click `Hackathon Race Demo` in the top bar, then click `Start Live Speed & Cost Race`)*
> **"In our live benchmark mode, a standard screenshot-based AI browser agent takes 34.2 seconds and $0.42 in tokens to parse a page. AgentGate Browser compiles the exact same page in under 200 milliseconds for $0.0004—over 100x faster and 99% cheaper."**

---

### [2:15 – 2:35] Built with Kiro (`/.kiro Specs & Hooks` Button)
*(Click the green `/.kiro Specs & Hooks` button in the bookmarks bar)*
> **"Finally, we built AgentGate Browser using Kiro's spec-driven workflow. Right inside the browser, you can inspect our `/.kiro/specs/`, steering rules, MCP config, and live Agent Hook execution logs that fire every time a tab navigates or the Safety Brake triggers. Thank you!"**

---

## Part 2: Copy-Paste Answers for the Kiroween Devpost Form

### Project Title
`AgentGate Browser — The AI-Native Headless Web Browser & UI Compiler`

### Tagline (Short Description)
`A headless Chromium web browser that compiles bloated websites into 98% smaller AI-ready pages in milliseconds—with a Permanent Default AI Bridge and a deterministic Safety Brake.`

### Category to Select on Kiroween
- **Primary Category:** `Frankenstein` *(Stitching together two incompatible worlds—bloated human HTML/DOM and fast, deterministic AI agents—into one seamless AI Browser)* OR `Skeleton Crew`
- **Bonus Prizes to Check:** `Best Startup Project ($10,000)` and `Student Prize ($1,500)`

### "How We Used Kiro" (Copy-Paste into the Devpost Kiro Question)
> We used Kiro's spec-driven development workflow (`/.kiro/specs/`), Steering documents (`/.kiro/steering/architecture.md`), Agent Hooks (`/.kiro/hooks/`), and MCP configuration (`/.kiro/mcp/mcp.json`) as the backbone of AgentGate Browser:
> 1. **Kiro Specs (`/.kiro/specs/`):** Before writing the compiler, we defined three modular specifications (`agentgate-translator.md`, `headless-browser-compiler.md`, and `permanent-ai-bridge.md`) to structure how Playwright Chromium HTML is stripped and compiled into 3 Takeout Bag formats (`Simple List`, `Code Data / JSON`, and `Spreadsheet / CSV`) while achieving >90% token compression.
> 2. **Kiro Agent Hooks (`/.kiro/hooks/`):** We implemented two event-driven Kiro hooks (`on-tab-navigate.hook.json` and `on-high-risk-action.hook.json`) that automatically sync all open browser tabs to `.kiro/live-browser-state.json` for the user's Permanent Default AI and freeze checkout/payment actions via our Safety Brake.
> 3. **Kiro Steering (`/.kiro/steering/architecture.md`):** Enforced strict plain-English UI rules, high-contrast developer aesthetics, and zero-trust financial action interception across every component.
