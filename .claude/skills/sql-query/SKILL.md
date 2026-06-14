---
name: sql-query
description: Write, validate, and deploy a SQL Query Activity in Automation Studio (Salesforce MCE).
argument-hint: "[describe the data you need — source DEs, filters, output DE]"
context: fork
agent: automation-agent
---
Run as the **automation-agent**. 1) Fetch schemas for all source DEs. 2) Confirm the (non-sendable)
target output DE. 3) Draft SFMC-dialect SQL (no CTEs → nested derived tables; `TOP n` not `LIMIT`)
with inline comments. 4) Validate. 5) Create the activity only after explicit confirmation.
