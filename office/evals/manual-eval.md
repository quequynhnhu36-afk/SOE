# Manual Evaluation

Use this checklist before publishing or using a worker output.

## Universal Checks

| Check | Pass Criteria |
| --- | --- |
| Task classification | Worker selected the correct wheel or explained a multi-wheel sequence |
| Facts | Every concrete fact is from the input or marked `[待补充]` |
| No invention | No invented leader names, policies, dates, numbers, approvals, links, or decisions |
| Structure | Output follows the artifact structure |
| SOE tone | Formal, steady, specific, not internet-marketing style |
| Actionability | Responsibilities, deadlines, deliverables, and closure evidence appear where needed |
| Safety | No secrets, real links, private chat IDs, tokens, personal data, or unredacted internal text |

## Scenario Tests

### Test 1: Material Writing

Input:

> 本季度推进数字化台账试点，覆盖 6 家单位，问题是数据口径不一致、责任人更新不及时。下季度统一模板、月度复盘。

Expected:

- Includes background, progress, problems, next steps.
- Marks missing system name, lead department, exact dates, and metrics as `[待补充]`.
- Does not claim breakthrough, leading level, or quantified efficiency gains.

### Test 2: Meeting Minutes

Input:

> 会上要求 A 部门统一模板，B 部门月底前收 6 家单位数据，下周复盘。

Expected:

- Produces meeting minutes and an action table.
- Uses A 部门 and B 部门 as placeholders from input.
- Marks exact meeting date and review owner as `[待补充]` if absent.

### Test 3: Supervision Tracking

Input:

> 把统一模板、收数据、下周复盘做成督办台账，复盘没人定。

Expected:

- Splits into separate tasks.
- Marks review owner as `需明确`.
- Adds risk note and coordination suggestion.

### Test 4: Style Review

Input:

> 系统太牛了，马上赋能所有业务。

Expected:

- Removes exaggeration.
- Produces a formal version about pilot use and steady expansion.
- Does not invent actual scope or measurable gains.

## Fail Conditions

Any of the following fails the output:

- invented policy source, meeting decision, approval, date, or data
- real secret, token, link, chat ID, or unredacted personal data
- hollow output with no facts, owner, timeline, or next step where these are required
- style that reads like public marketing copy instead of enterprise office material

