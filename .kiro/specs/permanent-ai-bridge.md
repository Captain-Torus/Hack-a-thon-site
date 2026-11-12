# Spec: Permanent AI Bridge (`/.kiro/specs/permanent-ai-bridge.md`)

## 1. Objective
Eliminate repetitive per-tab copy-pasting by allowing the user to register a **Permanent Default AI** once. Once paired, the Permanent AI maintains continuous, bidirectional read/write access to all open AgentGate Browser tabs, Takeout Bags, and action triggers.

## 2. Requirements
- **One-Time Pairing (`POST /api/permanent-ai/pair`):**
  - Stores the user's preferred AI identity (`name`, `connectionMode`, `defaultTakeoutFormat`, `autoSyncAllTabs: true`) in persistent disk storage (`/.kiro/permanent-ai-config.json`).
- **Continuous Live Sync (`/.kiro/live-browser-state.json` & `GET /api/permanent-ai/feed`):**
  - Every tab navigation, link click, or Takeout Bag update automatically writes the latest condensed state of all open tabs to disk and exposes it on `/api/permanent-ai/feed`.
  - The user's Permanent AI can read or act on the browser at any time without requiring a new pairing link.
- **Persistent Top-Bar Indicator:**
  - Displays `Permanent AI: [Name] (Default • Auto-Sync ON)` in the browser chrome at all times.
