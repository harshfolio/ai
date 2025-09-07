
---
tags:
  - status/evergreen
  - type/resource
  - topic/prompt-engineering
---


> [!NOTE] A word of caution
> This knowledge is upto date till the last edited time, This is a super dynamic space which keeps changing. Written down ideas & techniques may get outdated as models become better.
> 
> However,  _Design with Intent. Think in Systems._ and you'll be fine

# Core Principles
1. **Precision Over Poetry**
	1. Avoid vague, flowery language. Be explicit about what you want — format, tone, length, exclusions. Think like a spec, not a slogan.
2. **Iterate Like a Builder**
	1. Don’t expect the first draft to be perfect. Prompt engineering is iterative: test, revise, tighten.
	2. The first output is scaffolding, not the solution.
3. **Start With Intent**
	1. What’s this for? Who’s it for? Where will it be used? Good prompts work backwards from the real-world use case.
4. **Structure Like a System**
	1. Separate the **what** from the **how**. Use sections, bullet points, or JSON-style structure to reduce ambiguity and increase reusability.
	2. Think in templates and prompt blocks. If it works once, you should be able to use it 100 times.
5. **Design for Determinism**
	1. Determinism means your prompt behaves **predictably**. You’re not leaving it up to luck. Especially when building repeatable workflows (e.g., agents, automations, APIs), you want **consistency over creativity**.
	2. The **enemy of determinism** is
		1. Open-ended instructions: "Make this sound better."
		2. Unspecified constraints: "Summarize this" (without length/tone guidance)
		3. Too much creativity for the task
		4. Model randomness (temperature settings, etc.)
	3. If you want prompts to be deterministic
		1. Be explicit: Format, tone, exclusions, structure
		2. Use examples: Anchor outputs with sample completions
		3. Control temperature: Set to 0 or low for programmatic use
		4. Avoid underspecification: If anything’s left to interpretation, clarify it

# Bonus
- If you find yourself using a format repeatedly, codify it:

```
{
  "input": "text string",
  "task": "summarization",
  "constraints": {
    "length": "max 3 lines",
    "tone": "analytical",
    "format": "bullet list"
  }
}

```

---
Date: 2025-07-14