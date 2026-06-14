---
name: content-create
description: Create or update Content Builder assets — HTML emails, templates, SMS assets, content blocks (Salesforce MCE).
argument-hint: "[asset type: email | template | sms | asset] [name or description]"
context: fork
agent: content-agent
---
Run as the **content-agent**. Confirm asset type, target folder, and all content details. For email:
subject, preheader, HTML, sender profile. Use null-safe AMPScript only (no SET-from-comparison); host
images via the asset API → CDN URL. For updates, show current vs proposed diff before applying.
