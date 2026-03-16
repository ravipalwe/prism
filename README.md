# PRISM — People Research & Insight System for Makers

An AI agent skill that gives Claude (and other AI coding assistants) the ability to generate professional UX research deliverables grounded in **industry-standard UX research methodology**.

Built by **[Ravi Palwe](mailto:ravi.palwe@gmail.com)** — 19+ years in Product Design leadership at Bank of America, Capital One, and Capgemini.

## What It Does

| Deliverable | What You Get |
|---|---|
| **User Personas** | 3–5 research-backed personas with goals, behaviors, pain points, motivations, context of use, and design implications |
| **Journey Maps** | Phase-by-phase experience maps with emotional arcs, touchpoints, and prioritized opportunities |
| **Interview Synthesis** | Cross-participant findings with evidence strength ratings, direct quotes, themes, and recommendations |
| **Usability Test Plans** | Complete plans with research questions, task scenarios, metrics, participant criteria, and timelines |

### Financial Services Layer (Optional)

Built-in support for fintech, banking, payments, insurance, and wealth management. Adds trust signals, compliance friction (KYC, AML, PCI-DSS), financial anxiety analysis, and regulatory touchpoints to every deliverable.

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
├── SKILL.md                          # Main skill instructions
├── package.json                      # npm metadata
├── LICENSE.txt                       # MIT license
├── references/                       # Detailed generation guides
│   ├── PERSONA-GUIDE.md              # Persona template & research methodology
│   ├── JOURNEY-MAP-GUIDE.md          # Journey map template & guidelines
│   ├── SYNTHESIS-GUIDE.md            # Interview synthesis methodology
│   ├── TEST-PLAN-GUIDE.md            # Usability test plan template
│   ├── FINSERV-LAYER.md              # Financial services additions
│   └── QUALITY-CHECKLIST.md          # Pre-delivery validation checks
├── scripts/
│   └── validate-output.js            # Output validator (zero dependencies)
└── assets/
    └── research-brief-template.json  # Structured input schema
```

## Usage Examples

Just describe what you need in natural language:

- *"Create user personas for a mobile banking app targeting Gen Z users"*
- *"I have interview notes from 6 users about our onboarding flow — synthesize them"*
- *"Write a usability test plan for our new peer-to-peer payments feature, we launch in 6 weeks"*
- *"Map the customer journey for opening a brokerage account, include the financial services layer"*

The skill automatically identifies which deliverable you need, classifies your input fidelity (raw data vs. brief), and follows the relevant research template.

## Validate Outputs

```bash
node scripts/validate-output.js outputs/personas.md persona
node scripts/validate-output.js outputs/interview-synthesis.md synthesis
node scripts/validate-output.js outputs/usability-test-plan.md test-plan
node scripts/validate-output.js outputs/journey-map-maya.md journey-map
```

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
# prism
