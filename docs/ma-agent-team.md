# M&A Expert Agent Team

There are 15 specialist agents, set up as Claude Code subagents in [`.claude/agents/`](../.claude/agents/). Each one acts as one of the expert roles from [m-and-a-app-expert-roles.md](./m-and-a-app-expert-roles.md), tuned for GES's acquisition program (see [ges-company-research.md](./ges-company-research.md)).

## The team

| # | Agent | Role | Answers |
|---|---|---|---|
| 1 | `corp-dev-director` | Deal lead / IC chair | Should we do this deal? (frames the deal, writes the IC memo) |
| 2 | `investment-banker` | M&A advisor | What should we bid, and how should we structure it? |
| 3 | `pe-operating-partner` | Sponsor view | Does this create value for the platform and Truelink? |
| 4 | `strategy-consultant` | Strategy & screening | Is it a strategic fit? Who else should we look at? |
| 5 | `events-industry-expert` | Industry SME | Is the book of shows, venues and labor any good? |
| 6 | `valuation-analyst` | Financial modeling | What is it worth? (DCF, comps, LBO, sensitivities) |
| 7 | `qoe-accountant` | Quality of earnings | Are the earnings real? NWC peg, debt-like items |
| 8 | `ma-tax-advisor` | Tax structuring | Best structure? Hidden tax exposure? |
| 9 | `ma-attorney` | Transaction counsel | Legal risks, deal terms, closing conditions |
| 10 | `labor-employment-counsel` | Labor & unions | CBAs, pension withdrawal liability, worker classification |
| 11 | `commercial-contracts-counsel` | Contract review | Does the revenue survive a change of control? |
| 12 | `antitrust-counsel` | Competition law | Filings needed? Regulatory risk in competitor deals? |
| 13 | `commercial-diligence-analyst` | Customer & market | Will customers stay? Is the forecast credible? |
| 14 | `people-diligence-specialist` | HR / talent | Who must we keep, and what does it cost? |
| 15 | `integration-lead` | Post-merger integration | Are the synergies real? Day 1 and 100-day plan |

Roles from the full list that are **not** agents yet (good Phase 2 candidates): IT/cyber diligence, data privacy counsel, IP counsel, international counsel, FP&A, technical accounting, operations/supply chain, risk management, ESG.

## How it works

Every agent follows the same rules:
- It reads the GES research for acquirer context.
- It works from the deal folder (`deals/<target-slug>/inputs/`) and public information only, and it **never invents figures**.
- It keeps deal data confidential: no confidential details go into web searches.
- It writes its analysis to `deals/<target-slug>/analysis/<agent-name>.md` in a standard format: **verdict 🟢/🟡/🔴**, findings, risks, data requests, and the items that need professional sign-off.

Subagents can't call other subagents, so the **main Claude Code session acts as the orchestrator**. It runs the specialists, often in parallel, and then hands their outputs to `corp-dev-director` to write the IC memo.

## Typical workflow

1. **Set up the deal folder.** Copy `deals/_template/` to `deals/<target-slug>/` and put the teaser, CIM, financials, contracts, etc. in `inputs/`.
2. **Frame the deal.** For example: *"Use the corp-dev-director agent to frame the deal and build a diligence plan for deals/acme-expo."*
3. **Run the specialists.** For example: *"Run the specialists from the diligence plan in parallel on deals/acme-expo."* Or call one directly: *"Use the qoe-accountant agent on deals/acme-expo."*
4. **Synthesize.** For example: *"Use the corp-dev-director agent to write the IC memo for deals/acme-expo."*
5. **After signing,** for example: *"Use the integration-lead agent to build the 100-day plan."*

You can also run agents with no specific target:
- *"Use the strategy-consultant agent to screen association marketing agencies in the US."*
- *"Use the antitrust-counsel agent to check current HSR thresholds."*

Type `/agents` in Claude Code to see and manage the agents.

## Customizing

Each agent is a Markdown file with YAML frontmatter:
- `name`: the agent's identifier
- `description`: tells Claude when to use the agent
- `tools`: which tools the agent may use
- `model`: which model it runs on

The body of the file is the agent's system prompt. Edit the body to change the agent's expertise or output format.

## Caveat

These agents support executive decisions. They do **not** replace licensed attorneys, CPAs, tax advisors or bankers. Every legal, tax and valuation conclusion needs professional sign-off before anyone acts on it.
