# AgentGate Core Specification (`/.kiro/specs/agentgate-translator.md`)

## 1. System Overview
AgentGate is a bidirectional Headless UI Compiler and Fast-Track Gate for autonomous AI agents. Instead of forcing LLM agents to parse 100,000+ tokens of bloated human HTML/CSS or rely on high-latency visual screenshots, AgentGate compiles live web interfaces into deterministic, low-token **Agentic Action Schemas** (typically 150–400 tokens) and maps agent action invocations back to the underlying web targets.

## 2. Core Capabilities
- **Inbound UI Compilation (Human UI -> Condensed AI-UI):**
  - Strips scripts, trackers, decorative DOM wrappers, and stylesheets.
  - Extracts the semantic Accessibility Tree (headings, structured data tables, interactive inputs, forms, and action triggers).
  - Intercepts embedded JSON-LD, Next.js/SSR hydration state (`__NEXT_DATA__`), and API endpoints.
- **Dual Configuration Modes:**
  - **Manual Gate Setup (Human-Defined):** Human specifies target URL(s), extraction layers, safety guardrails, and output formatting.
  - **Self-Service Auto-Configuration (AI-Defined):** AgentGate exposes a meta-configuration endpoint (`/api/gates/auto-configure`) allowing an autonomous agent to inspect the gate creation form, define its own target URLs and extraction flags, and provision a dedicated gate on the fly.
- **Instant Memory Cache:**
  - Caches compiled UI schemas and selector maps per URL hash for sub-20ms repeat execution.
- **Safety Brake Guardrail:**
  - Intercepts destructive or financial actions (`checkout`, `purchase`, `pay`, `delete`, `remove`, `transfer`) and places them into a `PENDING_HUMAN_APPROVAL` hold queue until explicitly approved or rejected by the human operator.
- **Takeout Bag Serializer:**
  - Exports condensed state in `json`, `bullets` (ultra-condensed Markdown), or `csv` table format.
- **Difficulty-Weighted Gate Credits:**
  - `1 Credit`: Instant Memory cache hit.
  - `5 Credits`: Cold live website compilation + JSON state extraction.
  - `15 Credits`: Multi-step action execution + Safety Brake verification.
