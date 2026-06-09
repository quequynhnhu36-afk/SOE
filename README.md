# SOE Worker SOPs

Public, sanitized worker wheels for state-owned enterprise office work.

This repository treats a worker skill as a Markdown SOP package. A single Markdown file can be the minimum viable wheel, but a reliable worker wheel should include an entry SOP, task-specific wheels, reusable templates, sanitized examples, and simple evaluation checks.

## First Domain

`office/` is the first domain. It supports SOE office workers handling:

- material writing
- meeting minutes
- requests and reports
- supervision tracking
- information briefings
- style review

## How Workers Use This

1. Read [`office/SOP.md`](office/SOP.md).
2. Classify the task and select one wheel under [`office/wheels/`](office/wheels/).
3. Use templates under [`office/templates/`](office/templates/) when the user requests a concrete artifact.
4. Run the quality checks in [`office/evals/manual-eval.md`](office/evals/manual-eval.md) before returning final output.

## Public Boundary

This is a public repository. Do not commit:

- real leader names, phone numbers, email addresses, chat IDs, Feishu links, meeting transcripts, internal screenshots, or approval records
- ECS, OpenClaw, Lark, GitHub, model provider, or dashboard tokens
- company secrets, internal policy files, unpublished business numbers, contract terms, or personal data
- unredacted user prompts copied from production conversations

Use placeholders such as `[单位名称]`, `[负责人]`, `[金额]`, `[时间]`, `[链接]`, and `[待补充数据]`.

## Writing Principle

SOE office writing should be steady, accurate, concrete, and executable. The worker must not invent facts, policies, data, leaders' statements, meeting decisions, or regulatory sources.

Good outputs connect:

- superior requirements
- enterprise context
- concrete work facts
- problems and risks
- responsibility and timeline
- closure evidence

## Repository Status

Version 0.1 focuses on Markdown SOPs for worker consumption. It intentionally does not include Codex `SKILL.md` metadata. A Codex-compatible layer can be added later under `codex-skills/`.

