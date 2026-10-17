<div align="right">

**[English](README.md)** · [简体中文](README.zh-CN.md)

</div>

# legal-ai-agent-research

Research and an implementation blueprint for an accessible legal AI agent — a near-zero-cost plan for a student team.

<sub>HTML · research/ and report/</sub>

---

## The premise

Legal advice is expensive and unevenly distributed. A student team cannot fund a law firm's tooling, so the question this research addresses is narrower: **what can be built for close to nothing, that is still genuinely useful?**

The answer shapes everything downstream. It rules out fine-tuned models, dedicated infrastructure and anything requiring a licence to operate. What remains is a narrow agent over public statute and procedure, with clear limits on what it will answer.

## Structure

```
research/    raw investigation — sources, prior art, legal constraints
report/      conclusions drawn from it
```

Raw findings stay separate from the conclusions. A conclusion can be re-examined against the evidence that produced it, and the evidence does not get rewritten to fit a later argument.

## What the report covers

- Which legal questions are answerable from public sources, and which are not
- Where the cost floor actually sits (hosting, model calls, data)
- The compliance boundary — what such a tool may and may not claim to do
- A build order for a small team

## Scope

This is research and a blueprint, not a deployed service. Legal conclusions carry jurisdiction limits that a general-purpose tool cannot paper over, and the report says so rather than glossing it.

## License

MIT
