# Art of War — Business Strategy DSS

Sun Tzu's 13 chapters, translated into a decision support system for competitive business situations. Not motivational. Diagnostic.

Works as a Claude Code skill or as a portable system prompt you can drop into ChatGPT, Gemini, Perplexity, Mistral, Copilot, or any LLM with a system message field.

---

## What it is

Most "Sun Tzu for business" content is motivational. This is not that.

Each chapter becomes a diagnostic framework with specific inputs and specific outputs. You don't use this to feel inspired. You use it when you're facing an actual competitive situation and need a structured way to think it through.

The 13 frameworks cover:

- Situation assessment: scoring five strategic factors and seven competitive comparators before any move
- Resource economics: when to sustain a campaign and when to stop
- Competitive strategy hierarchy: disrupt their plans before they execute, or work down to direct confrontation
- Defensive positioning: build invincibility before seeking victory
- Force composition: combining direct and indirect competitive moves
- Market gap analysis: where competitors are structurally weak or absent
- Positional maneuvering: gaining high ground through indirect routes
- Adaptive doctrine: which engagements to refuse, and the five command faults that cause strategic failure
- Signal reading: interpreting competitor behavior from indirect signs
- Terrain classification: six market environment types, each requiring a different response
- Situation mapping: nine competitive positions, each with its own doctrine
- Disruption vectors: five ways to attack a competitor's ecosystem
- Intelligence architecture: five source types, and why primary intelligence always beats inference

---

## How to use it

### In Claude Code

The skill installs to `~/.claude/skills/art-of-war-dss/SKILL.md`. Once there, you can invoke it:

```
/art-of-war-dss
```

Or trigger it naturally by describing a competitive situation in your conversation with Claude.

### In any other LLM

Copy the system prompt from `SKILL.md` (the section labeled "Model-Agnostic System Prompt") and paste it as your system message. Works with:

- ChatGPT (system message in the API, or custom instructions)
- Gemini (system instruction field)
- Perplexity (custom system prompt in settings)
- Mistral, Llama, Cohere, or any model with a system prompt field
- Open WebUI, LM Studio, or any local model interface

### Example prompts

```
Run a full Art of War assessment on this situation: [describe your competitive situation]
```

```
Apply the Nine Situations framework to our current market position.
```

```
We're in a pricing war with a larger competitor. Advise me using the Waging War and Attack by Stratagem frameworks.
```

```
Use the Terrain chapter to evaluate whether we should enter the enterprise segment.
```

---

## Installation

### Clone the repo

```bash
git clone https://github.com/asaulyuk/art-of-war-dss.git
cd art-of-war-dss
```

### Install as a Claude Code skill

```bash
mkdir -p ~/.claude/skills/art-of-war-dss
cp SKILL.md ~/.claude/skills/art-of-war-dss/SKILL.md
```

Restart Claude Code. The skill appears automatically.

### Use as a system prompt

Copy the contents of the "Model-Agnostic System Prompt" section in `SKILL.md`. Paste into any LLM's system message field.

---

## The 13 frameworks at a glance

| Chapter | Framework | Use when |
|---|---|---|
| 1. Laying Plans | Strategic Assessment | Before any major move |
| 2. Waging War | Resource Economics | Evaluating campaign duration and cost |
| 3. Attack by Stratagem | Competitive Strategy Hierarchy | Choosing how to compete |
| 4. Tactical Dispositions | Defensive Positioning | Building sustainable advantage |
| 5. Energy | Force Composition | Designing your competitive attack |
| 6. Weak Points and Strong | Market Gap Analysis | Finding where to attack |
| 7. Maneuvering | Positional Strategy | Gaining high ground indirectly |
| 8. Variation in Tactics | Adaptive Doctrine | Knowing what NOT to do |
| 9. Army on the March | Signal Reading | Interpreting competitor behavior |
| 10. Terrain | Environment Classification | Before entering a new market |
| 11. Nine Situations | Position Mapping | Identifying your strategic situation type |
| 12. Attack by Fire | Disruption Vectors | Targeting competitor vulnerabilities |
| 13. Use of Spies | Intelligence Architecture | Building your intelligence function |

---

## Design decisions

Porter, Blue Ocean, and BCG matrices were built for relatively stable competitive environments. Sun Tzu was built for situations where the opponent adapts to you, resources run out, and prolonged engagement compounds cost. That's closer to what most markets actually look like.

Strategy shouldn't be a Claude feature. The same frameworks should work in Perplexity for quick research, ChatGPT for team discussions, or a local model for sensitive work that shouldn't touch external APIs. The model-agnostic system prompt in `SKILL.md` handles this.

The difference between a persona and a DSS matters. "You are Sun Tzu" generates quotes. A decision support system takes specific inputs and returns ranked options. When you're making a real call, you need the second thing.

---

## Source

Sun Tzu, *The Art of War*, translated by Lionel Giles (1910). Public domain via Project Gutenberg.

Business framework synthesis by Marko Asaulyuk.

---

## License

MIT — see [LICENSE](LICENSE).
