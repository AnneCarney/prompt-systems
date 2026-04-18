# Prompt Systems

**Reusable prompt engineering frameworks for content, marketing, data, and workflow automation.**

A collection of production-grade system prompts designed to be dropped into Claude, ChatGPT, Gemini, or any capable LLM and produce consistent, high-quality output. Each framework is scoped to a specific job, structured to accept structured input, and tuned for reliability over cleverness.

---

## Frameworks

| Framework | Purpose | Input Type |
|---|---|---|
| [`content-generator`](./content-generator) | SEO-optimized long-form content from a structured brief | Content brief (topic, audience, keywords, structure) |
| [`campaign-builder`](./campaign-builder) | Platform-tailored social content from a single campaign brief | Campaign brief (objective, audience, message, platforms) |
| [`data-analyst`](./data-analyst) | Structured data analysis producing actionable insights | Dataset + analysis question |
| `knowledge-base-architect` | Organize raw knowledge into AI-ready structured sources | Document set + target use case |
| `project-instructions-builder` | Generate Claude Project instructions from a goal statement | Goal + context + constraints |

> `knowledge-base-architect` and `project-instructions-builder` are tracked here and will be added as their frameworks stabilize.

---

## Philosophy

**Prompts are infrastructure.**

A prompt isn't a clever sentence. It's the interface contract between a human process and a language model. The same way an API contract defines what inputs a service accepts and what outputs it guarantees, a production prompt defines what brief an operator supplies and what artifact the model returns.

Treating prompts as infrastructure means:

- **They are versioned.** Every change to a prompt is tracked. You know which version produced which output.
- **They are tested.** Before deployment, prompts are run against a fixed set of representative inputs and outputs are evaluated for quality.
- **They have explicit input formats.** Operators don't freestyle. They fill out a structured brief. This dramatically improves consistency.
- **They have explicit output formats.** The artifact returned is predictable in structure, even if creative in content.
- **They fail gracefully.** When inputs are incomplete or contradictory, the prompt surfaces the gap instead of guessing.
- **They are reusable.** One well-built prompt replaces hundreds of ad-hoc chat sessions.

The organizations treating prompts this way are the ones getting durable leverage from AI. The ones writing prompts like tweets are getting inconsistent output and blaming the model.

---

## Folder Structure

