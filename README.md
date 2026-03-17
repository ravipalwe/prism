# PRISM — People Research & Insight System for Makers

An AI agent skill with two modules: **UX Research** and **UI Design**. From research insight to design specification — grounded in industry-standard methodology.

Built by **[Ravi Palwe](mailto:ravi.palwe@gmail.com)** — 19+ years in Product Design leadership in Financial Services.

## What It Does

### Module 1: UX Research

| Deliverable | What You Get |
|---|---|
| **User Personas** | 3–5 research-backed personas with goals, behaviors, pain points, motivations, context of use, and design implications |
| **Journey Maps** | Phase-by-phase experience maps with emotional arcs, touchpoints, and prioritized opportunities |
| **Interview Synthesis** | Cross-participant findings with evidence strength ratings, direct quotes, themes, and recommendations |
| **Usability Test Plans** | Complete plans with research questions, task scenarios, metrics, participant criteria, and timelines |

### Module 2: UI Design

| Deliverable | What You Get |
|---|---|
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

## Project Structure

```
prism/
├── SKILL.md                              # Main skill instructions (both modules)
├── package.json                          # npm metadata
├── LICENSE.txt                           # MIT license
├── references/                           # Detailed generation guides
│   ├── PERSONA-GUIDE.md                  # Persona template & research methodology
│   ├── JOURNEY-MAP-GUIDE.md              # Journey map template & guidelines
│   ├── SYNTHESIS-GUIDE.md                # Interview synthesis methodology
│   ├── TEST-PLAN-GUIDE.md               # Usability test plan template
│   ├── PHILOSOPHY-GUIDE.md               # Design philosophy methodology
│   ├── TOKEN-GUIDE.md                    # Design token system template
│   ├── COMPONENT-GUIDE.md                # Component specification template
│   ├── LAYOUT-GUIDE.md                   # Layout system template
│   ├── INTERACTION-GUIDE.md              # Interaction & motion spec template
│   ├── CANVAS-GUIDE.md                   # Visual artifact creation guide
│   ├── FINSERV-LAYER.md                  # Financial services research additions
│   ├── FINSERV-UI-LAYER.md               # Financial services UI design additions
│   └── QUALITY-CHECKLIST.md              # Pre-delivery validation checks
├── scripts/
│   └── validate-output.js                # Output validator (zero dependencies)
└── assets/
    └── research-brief-template.json      # Structured input schema
```

## Usage Examples

Just describe what you need in natural language:

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

The skill identifies which module and deliverable you need, classifies your input fidelity, and follows the relevant template.

## Cross-Module Flow

Research deliverables feed design deliverables:

| Research Output | Feeds Into |
|---|---|
| Personas | Emotional targets in design philosophy, accessibility personas |
| Journey Maps | Key moment identification, state design, flow prioritization |
| Interview Synthesis | Pain point → design solution mapping |
| Usability Test Plans | Component testing criteria, interaction success metrics |

## Supported Platforms

Works with any AI assistant that supports the Agent Skills specification:

- Claude Code
- Cursor
- Windsurf
- Codex CLI
- Continue
- Gemini CLI
- And more

## Benchmark Results

Tested across 3 eval scenarios (personas, interview synthesis, usability test plan):

| Metric | With PRISM | Without PRISM | Delta |
|---|---|---|---|
| **Pass Rate** | 100% | 36% | **+64%** |
| **Avg Tokens** | 55K | 47K | +8K |
| **Avg Time** | 337s | 304s | +33s |

PRISM adds modest cost (~33 seconds, ~8K tokens) for a **64% quality improvement** on research methodology compliance, evidence-based structure, and actionable recommendations.

## License
MIT

