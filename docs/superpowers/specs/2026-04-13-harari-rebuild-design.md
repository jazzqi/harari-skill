# Harari Skill Nuwa Rebuild Design

## Problem

`jazzqi/harari-skill` already has a usable Harari-shaped skeleton, but it is still below the recent Nuwa rebuild standard used in newer repos. The current version is strong on headline concepts, but weaker on evidence density, research decomposition, research-first answering behavior, and explicit treatment of Harari's internal tensions and external criticism.

The rebuild should produce a self-contained, research-backed `harari-perspective` that is broader than a quote collection and more reliable than a macro-history caricature.

## Rebuild Goal

Create a full Nuwa-style rebuild of `harari-skill` with:

1. Comprehensive characterization of Yuval Noah Harari as a thinker
2. Output emphasis on:
   - civilization-scale history
   - imagined orders / intersubjective reality / narrative power
   - information networks, language, and AI
3. Stronger evidence chain from research files to final skill behavior
4. A research-first protocol for fact-dependent questions
5. Honest boundaries around simplification, prediction, and disciplinary limits

## Scope

### In scope

- Rebuild `SKILL.md`
- Rebuild `README.md`
- Rebuild `examples/demo-conversation.md`
- Rebuild `references/research/01-06.md`
- Refresh the repo so its packaging matches newer Nuwa-style skills

### Out of scope

- Creating a separate Harari theme skill outside this repository
- Translating entire books or reproducing copyrighted long passages
- Building automation scripts unless they are clearly needed for the rebuild

## Source Strategy

This rebuild will use full web research with first-party and long-form sources prioritized.

### Highest-priority sources

1. Harari's books:
   - *Sapiens*
   - *Homo Deus*
   - *21 Lessons for the 21st Century*
   - *Nexus*
   - important supporting material from *Unstoppable Us* if useful
2. Long interviews / podcasts / lectures:
   - TED
   - Sam Harris
   - Lex Fridman
   - major keynote and policy appearances
3. Harari's essays, public talks, policy testimony, and official pages
4. Serious outside criticism and review material

### Lower-priority sources

- Short social snippets used only for expression/style confirmation

### Excluded or de-emphasized

- Thin secondary summaries
- generic quote sites
- low-trust reposted commentary

## Deliverables

### 1. Research layer

`references/research/` will contain:

- `01-writings.md` — books, essays, repeated claims, concept inventory
- `02-conversations.md` — interview behavior, improvisation, refusal patterns, reframing
- `03-expression-dna.md` — phrasing, structure, rhetorical habits, level of certainty
- `04-external-views.md` — praise, criticism, blind spots, scholarly objections
- `05-decisions.md` — major public choices, positioning, partnerships, high-signal actions
- `06-timeline.md` — career stages, turning points, recent 12-month developments

### 2. Skill layer

`SKILL.md` will include:

- role rules
- research-first Agentic Protocol
- identity card
- 3-7 core mental models
- 5-10 decision heuristics
- expression DNA
- internal tensions
- values / anti-patterns
- honest boundaries
- source summary

### 3. Packaging layer

- `README.md` aligned with the rebuilt skill
- `examples/demo-conversation.md` with at least one true research-first scenario

## Design Approach Options

### Option A — Full Nuwa rebuild **(chosen)**

Re-run six-dimensional research and rewrite all major artifacts.

**Why chosen:** the user explicitly wants a non-shallow rebuild, and Harari is too broad a figure for a patch-only approach.

### Option B — Partial rebuild

Keep much of the current `SKILL.md`, but replace research and examples.

**Why rejected:** likely leaves behind old abstractions and weaker protocol design.

### Option C — Minimal patch

Edit only obvious gaps.

**Why rejected:** does not solve the "too simple" problem.

## Proposed Thinking Architecture

The rebuilt skill should frame Harari not just as "the macro-history guy," but as a thinker operating across four linked lenses:

1. **Species-scale cooperation through stories**
2. **Narrative power as a political and civilizational force**
3. **Information systems reshaping human agency**
4. **Meditative self-observation as a counterweight to narrative capture**

These lenses should allow the skill to answer both abstract and current-event questions without collapsing into generic futurism.

## Agentic Protocol Design

The new protocol should distinguish:

1. **Pure framework questions** — answer directly via Harari's mental models
2. **Fact-dependent questions** — research first, then interpret in Harari's frame
3. **Mixed questions** — gather current facts, then connect them to long-history patterns

The research step should inspect:

- what story / imagined order is operating
- what information network is shaping behavior
- who gains narrative power or data advantage
- what historical analogies are genuinely relevant
- what simplifications or unknowns limit confidence

## Error Handling and Boundaries

The rebuilt skill must avoid three common failure modes:

1. **Macro hand-waving** — sounding Harari-like without real structure
2. **Fake certainty** — predicting future outcomes too confidently
3. **Hagiography** — preserving his charm while hiding serious scholarly criticism

The skill should explicitly say when:

- the evidence is weak
- the issue is too technical for Harari's real expertise
- the analysis is a framework-based inference rather than a known public position

## Validation Plan

The rebuild will be judged by:

1. **Voice fidelity** — recognizably Harari, but not stitched from catchphrases
2. **Framework transfer** — can explain new cases with Harari-style reasoning
3. **Tension honesty** — includes criticisms of simplification and elite-platform contradiction
4. **Packaging consistency** — skill, README, examples, and research all agree

## Implementation Notes

- Preserve repo structure unless a clear Nuwa-standard adjustment is needed
- Keep copyright-safe paraphrase discipline
- Favor strong source attribution in research files over inflated claims in `SKILL.md`

