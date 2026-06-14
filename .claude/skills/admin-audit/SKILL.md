---
name: admin-audit
description: Read-only audit + subscriber lookup — channel subscription status, contact attributes, org config, account health check (Salesforce MCE).
argument-hint: "[email address | subscriber key | 'health-check']"
context: fork
agent: admin-agent
---
Run as the **admin-agent**. For a single subscriber: resolve SubscriberKey from the email first, then
check all channel statuses. For a health check: list lists, sender profiles, and send classifications,
then summarise as a markdown table. Read-only unless the user explicitly asks to update contact
attributes (which requires confirmation). Account-**user** lists are not accessible on this package.
