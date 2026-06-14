---
name: journey-design
description: Design, create, or manage a Journey Builder journey — entry sources, splits, waits, contact in/out (Salesforce MCE).
argument-hint: "[journey goal, entry type, activity steps]"
context: fork
agent: journey-agent
---
Run as the **journey-agent**. Gather journey name, entry source, goal, exit criteria, re-entry rules,
and the full activity sequence. Present the complete plan for review before any create call.
Random-split percentages must sum to 100; the control branch gets no send.
