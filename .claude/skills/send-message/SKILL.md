---
name: send-message
description: Send a transactional email, outbound SMS, or push to a specific contact — high-stakes, always confirms (Salesforce MCE).
argument-hint: "[channel: email | sms | push] [subscriber/contact key] [message or definition key]"
context: fork
agent: content-agent
---
Run as the **content-agent**. 1) Confirm channel, recipient identifier, and message/definition.
2) Check subscription/opt-in status for the channel. 3) Show a full send preview and require explicit
confirmation. NEVER send without explicit confirmation. (SMS/Push are 403/unprovisioned on this
instance — spec-only unless provisioning is confirmed.)
