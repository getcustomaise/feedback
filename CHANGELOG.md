# Customaise Changelog

All notable changes to the Customaise Chrome extension are documented here.

## [1.2.7] - May 2026

### Added
- **On-device AI in Chat.** Pick Gemini Nano in the Chat model selector to run prompts locally on your machine. Free, private, no API key. Best for short questions and lightweight tool calls; longer planning still uses cloud models. Requires Chrome 148+ on desktop.
- **`@grant CM_promptAI` for scripts.** UserScripts and AgentScripts can call on-device AI directly. Declare `@grant CM_promptAI` and call `await CM_promptAI(prompt, opts?)` from your code. Pass a JSON schema for structured output. Script input stays on the user's machine.

### Improved
- The in-browser AI Chat that builds scripts now reaches for the right Customaise grant (on-device AI, Chrome DevTools, bulletproof selectors) when your description fits one.

---

## [1.2.6] - May 2026

### Added
- **Full-page and any-tab screenshots.** Capture a whole scrollable page in one image, or screenshot any open tab without changing focus.
- **Chrome DevTools Access.** An opt-in control under Settings → Scripts that lets a script use Chrome DevTools on the pages it matches. Off by default, resets every Chrome restart, and a single switch turns it off for every script at once. Chrome shows its standard yellow banner while a session is active and clears when it ends.

### Improved
- AI agents open new tabs in the background while building scripts, so your current tab keeps focus.
- Script Management opens faster.

### Fixed
- Scripts that contain regular expressions now save correctly. Editor error markers point to the exact line.

---

## [1.2.5] - May 2026

### Fixed
- Minor stability and UI fixes.

---

## [1.2.4] - May 2026

### Fixed
- Minor stability fixes.

---

## [1.2.3] - May 2026

### Added
- **MCP Bridge is now free** for any signed-in Customaise user. 50 calls per day, 150 per week. Power User unlocks unlimited.
- **Marketplace Phase 1+2.** Browse the curated AgentScript catalogue and install community scripts directly from customaise.com. Publishers get a portal to ship their own.

---

## [1.2.0] - April 2026

### Added
- **AgentScripts.** A new kind of script. Instead of changing how a page looks, AgentScripts expose tools on the page that any connected AI agent can call on your behalf through WebMCP. Write once, call from Cursor, Claude Code, Codex, or any MCP-compatible editor.
- **Human-in-the-Loop approvals.** Sensitive tool calls pause and wait for your explicit OK. Approve right in the tab, or from your Account Portal on any signed-in browser including your phone.
- **Account Portal redesign.** Pending approvals, purchase history, and activity feed live in one place.

### Improved
- Many stability and polish fixes across script management, chat, and sync.

---

## [1.1.9] - April 2026

### Fixed
- Minor bug fixes and stability improvements.

---

## [1.1.8] - April 2026

### Fixed
- Minor bug fixes and underlying stability improvements.

---

## [1.1.7] - March 2026

### Added
- **Cloud Script Sharing.** Publish scripts to the community, subscribe to others, and manage everything from your Account Portal.
- **MCP Server.** Connect AI coding agents (Cursor, Claude Code, Codex, Windsurf, Kiro, Antigravity) directly to Customaise via `npx -y @customaise/mcp`. Script lifecycle, visual DOM targeting, browser context, and screenshots, all from your IDE. Power User plan required.
- **Visual DOM selection.** Pick elements in the browser and get bulletproof selectors auto-pushed to your IDE.

---

## [1.1.6] - March 2026

### Added
- Voice-to-Text input with live waveform and 21 languages.
- Browser Agent: AI that sees your screen and clicks, types, and navigates autonomously.
- Language preference for AI responses and voice input (Settings > Appearance).

### Fixed
- Minor fixes to panel spacing, imported script handling, and UI animations.

---

## [1.1.5] - March 2026

### Fixed
- Saved data and preferences now persist reliably across page reloads.

---

## [1.1.4] - March 2026

### Added
- Animated favicon: spins while AI is working, green when idle.
- Quick Actions toolbar with streamlined script controls.
- Redesigned script list with domain pills and tab counts.
- Split-screen extension settings window for side-by-side setup.
- Auth expiry alerts surface before session silently drops.
- What's New notification system with cascading dismissal.
- Support page with help resources and contact options.

### Improved
- AI broadcasts scoped per conversation, no more cross-chat bleed.
- Workflow recovery after reload and system-blocked plan states.
- AI page-vision reload guidance and stale-capture warnings.
- All Pages match-rule toggle with safer guard logic.

### Fixed
- Right-edge resize now correctly anchors the left side.
- Dropdown menus rendering and position-shift on open.
- Accordion spring animation snap glitch on expand/collapse.

---

## [1.1.3] - March 2026

### Added
- Platform Activity Feed with real-time event monitoring.
- Bring Your Own Key (BYOK) with per-model token breakdown.
- Smart Protect Engine for SPAs and native dark modes.

### Improved
- Welcome onboarding with split-screen Developer Mode setup.
- Glassmorphic UI overhaul across all panels and components.

### Fixed
- Dark mode blur restoration and thumbnail inversion.
