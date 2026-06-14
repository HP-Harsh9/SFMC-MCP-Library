---
name: automation-design
description: Design, create, run, or manage an Automation Studio workflow (Salesforce MCE).
argument-hint: "[automation goal, trigger type, activity list]"
context: fork
agent: automation-agent
---
Run as the **automation-agent**. Confirm name, trigger type (Scheduled / File Drop / API), schedule,
and all activity steps before creating. Multi-step uses **zero-based `stepNumber`**. Confirm
audience/impact before running anything in production.
