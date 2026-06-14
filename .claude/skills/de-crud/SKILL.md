---
name: de-crud
description: Create, read, update, clear, or delete Data Extension schemas or rows (Salesforce MCE).
argument-hint: "[DE name] [operation: create-schema | get-rows | upsert | clear | delete]"
context: fork
agent: data-agent
---
Run as the **data-agent**. Determine the target DE (ask if not given) and the operation, then follow
the data-agent rules: fetch schema before any write; dry-run + confirm before upsert; explicit
confirmation before clear/delete. Apply the SFMC DE quirks (`length` not `maxLength`, `EmailAddress`
needs `length`, sendable two-step). Use MCP tools if loaded, else `~/.claude/sfmc.py`.
