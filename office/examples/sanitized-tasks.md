# Sanitized Example Tasks

These examples are fictional and safe for a public repository.

## Example 1: Work Report

Input:

> 请根据要点写集团内部汇报：本季度推进数字化台账试点，覆盖 6 家单位，发现数据口径不一致、责任人更新不及时两个问题。下季度准备统一模板、建立月度复盘。

Expected behavior:

- Use `wheels/material-writing.md`.
- Include background, progress, problems, next steps.
- Do not invent completion rate or system name.
- Mark missing owner, system name, and detailed data as `[待补充]`.

## Example 2: Meeting Minutes

Input:

> 会上讨论了数字化台账，要求 A 部门统一模板，B 部门月底前收集 6 家单位数据，下周再复盘。

Expected behavior:

- Use `wheels/meeting-minutes.md`.
- Separate discussion from decisions.
- Generate an action table with owner, deadline, deliverable.
- Mark the next review meeting's exact date as `[待补充]`.

## Example 3: Supervision Tracking

Input:

> 帮我把会议定下来的统一模板、收数据、下周复盘做成督办台账。复盘责任人还没定。

Expected behavior:

- Use `wheels/supervision-tracking.md`.
- Split three tasks.
- Mark review owner as `需明确`.
- Add risk note: unclear review owner may affect closure.

## Example 4: Style Review

Input:

> 这个系统特别炸裂，直接把效率拉满，马上赋能全部业务。

Expected behavior:

- Use `wheels/style-review.md`.
- Replace exaggeration with steady SOE wording.
- Keep only supportable value.
- Do not add unprovided achievements.

