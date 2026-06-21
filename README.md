<div align="center">

![PRISM — People Research & Insight System for Makers](assets/prism-hero.png)

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE.txt)
[![Agent Skill](https://img.shields.io/badge/type-agent%20skill-7c3aed)](https://github.com/ravipalwe/prism)
[![Works with Claude Code · Cursor · Windsurf](https://img.shields.io/badge/works%20with-Claude%20Code%20·%20Cursor%20·%20Windsurf-1f6feb)](#supported-platforms)
[![Stars](https://img.shields.io/github/stars/ravipalwe/prism?style=social)](https://github.com/ravipalwe/prism/stargazers)

**An AI agent skill that takes you from research insight to design specification — grounded in industry-standard methodology.**

One plain-language prompt in, a research-backed deliverable out. Two modules: **UX Research** and **UI Design**.

</div>

---

## See It In Action

<!--
  Replace the line below with a 10–20s screen recording of one prompt producing one deliverable.
  Record a prompt in Claude Code -> a persona or design-token sheet rendering. Save to assets/demo.gif (or .mp4) and commit it.
  This is the single highest-impact thing you can add to this page.
-->

![PRISM generating a deliverable from a single prompt](assets/demo.gif)

### Example output

<!-- Run PRISM once, then drop real screenshots into assets/ named to match. Real captures beat mockups. -->

| Persona | Journey Map | Design Tokens | Canvas Artifact |
| :-----: | :---------: | :-----------: | :-------------: |

---

Built by **[Ravi Palwe](mailto:ravi.palwe@gmail.com)** — 19+ years in Product Design leadership in Financial Services. PRISM encodes that methodology into a skill, so the output reflects how a senior practitioner actually works, not a generic prompt.

## What It Does

### Module 1: UX Research

| Deliverable | What You Get |
| --- | --- |
| **User Personas** | 3–5 research-backed personas with goals, behaviors, pain points, motivations, context of use, and design implications |
| **Journey Maps** | Phase-by-phase experience maps with emotional arcs, touchpoints, and prioritized opportunities |
| **Interview Synthesis** | Cross-participant findings with evidence strength ratings, direct quotes, themes, and recommendations |
| **Usability Test Plans** | Complete plans with research questions, task scenarios, metrics, participant criteria, and timelines |

### Module 2: UI Design

| Deliverable | What You Get |
| --- | --- |
| **Design Philosophy** | Named aesthetic direction with vision, principles, emotional targets, and anti-patterns |
| **Design Tokens** | Complete color, typography, spacing, elevation, radius, and motion token system |
| **Component Specs** | Anatomy, states, behavior, responsiveness, accessibility, and Do/Don't for every component |
| **Layout System** | Grid, breakpoints, page templates, content regions, navigation patterns, and empty states |
| **Interaction Spec** | Motion principles, timing system, feedback patterns, transitions, gestures, and loading states |
| **Canvas Artifacts** | Visual design expressions as .pdf or .png — posters, infographics, brand identity pieces |

### Financial Services Layer (Optional)

Built-in support for fintech, banking, payments, insurance, and wealth management. Adds trust signals, compliance friction (KYC, AML, PCI-DSS), financial anxiety analysis, trust-specific design tokens, financial component patterns, and regulatory touchpoints to every deliverable.

## Install

### Automated (Recommended)

```bash
npx skills add ravipalwe/prism
```

### Manual

Add the path to `SKILL.md` to your `.claude/settings.json`:

```json
{
  "skills": ["path/to/prism/SKILL.md"]
}
```

## Quick Start

Install, then just describe what you need in plain language:

```
Create user personas for a mobile banking app targeting Gen Z users.
```

PRISM identifies the module and deliverable, classifies your input fidelity, and follows the relevant template.

## Usage Examples

**Research:**

- *"Create user personas for a mobile banking app targeting Gen Z users"*
- *"I have interview notes from 6 users about our onboarding flow — synthesize them"*
- *"Write a usability test plan for our new peer-to-peer payments feature"*
- *"Map the customer journey for opening a brokerage account, include the financial services layer"*

**Design:**

- *"Create a design system for a mobile banking app — calm, trustworthy, professional"*
- *"I need component specs for a payment confirmation flow"*
- *"Design tokens for a wealth management dashboard — include the financial services layer"*
- *"Generate a layout system for an insurance comparison app"*

## Cross-Module Flow

Research deliverables feed design deliverables:

| Research Output | Feeds Into |
| --- | --- |
| Personas | Emotional targets in design philosophy, accessibility personas |
| Journey Maps | Key moment identification, state design, flow prioritization |
| Interview Synthesis | Pain point → design solution mapping |
| Usability Test Plans | Component testing criteria, interaction success metrics |

## Benchmark Results

Tested across 3 eval scenarios (personas, interview synthesis, usability test plan):

| Metric | With PRISM | Without PRISM | Delta |
| --- | --- | --- | --- |
| **Pass Rate** | 100% | 36% | **+64%** |
| **Avg Tokens** | 55K | 47K | +8K |
| **Avg Time** | 337s | 304s | +33s |

PRISM adds modest cost (~33 seconds, ~8K tokens) for a **64% quality improvement** on research methodology compliance, evidence-based structure, and actionable recommendations.

## Supported Platforms

Works with any AI assistant that supports the Agent Skills specification:

- Claude Code
- Cursor
- Windsurf
- Codex CLI
- Continue
- Gemini CLI
- And more

## Project Structure

```
prism/
├── SKILL.md                              # Main skill instructions (both modules)
├── package.json                          # npm metadata
├── LICENSE.txt                           # MIT license
├── references/                           # Detailed generation guides
│   ├── PERSONA-GUIDE.md
│   ├── JOURNEY-MAP-GUIDE.md
│   ├── SYNTHESIS-GUIDE.md
│   ├── TEST-PLAN-GUIDE.md
│   ├── PHILOSOPHY-GUIDE.md
│   ├── TOKEN-GUIDE.md
│   ├── COMPONENT-GUIDE.md
│   ├── LAYOUT-GUIDE.md
│   ├── INTERACTION-GUIDE.md
│   ├── CANVAS-GUIDE.md
│   ├── FINSERV-LAYER.md
│   ├── FINSERV-UI-LAYER.md
│   └── QUALITY-CHECKLIST.md
├── scripts/
│   └── validate-output.js                # Output validator (zero dependencies)
└── assets/
    └── research-brief-template.json      # Structured input schema
```

## Contributing

Contributions are welcome. Good places to start:

- Add new deliverable templates or reference guides
- Extend the financial services layer (or add a new domain layer)
- Add eval scenarios to the benchmark
- Report gaps where output quality could improve

Open an issue or a pull request — they're acknowledged quickly.

## License

[MIT](LICENSE.txt)
