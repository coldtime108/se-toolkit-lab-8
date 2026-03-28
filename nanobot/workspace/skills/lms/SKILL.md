---
name: lms
description: Use LMS MCP tools for live course data
always: true
---

# LMS Skills

You have access to the following LMS MCP tools:

- `lms_health` – check backend health (returns item count)
- `lms_labs` – list all available labs with titles
- `lms_pass_rates` – get pass rates for a specific lab (requires lab ID)
- `lms_scores` – get scores for a lab
- `lms_completion_rate` – get completion rate for a lab
- `lms_groups` – get group performance for a lab
- `lms_timeline` – get submission timeline for a lab
- `lms_top_learners` – get top learners for a lab

When a user asks for scores, pass rates, completion, groups, timeline, or top learners without specifying a lab, first call `lms_labs` to retrieve available labs. If multiple labs exist, ask the user to choose one.

Use lab titles as user‑friendly labels.

Format numeric results nicely: percentages with one decimal, counts as integers.

Keep responses concise and informative.

If the user asks "what can you do?", explain your LMS tools and their purpose.
