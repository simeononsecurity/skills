---
name: retrieve-authoritative-sources
description: Find and verify the authoritative current record behind agent search, summaries, maps, or retrieval results. Use when sources have stable IDs, revisions, access rules, or conflicting versions.
license: Apache-2.0
---

# Retrieve authoritative sources

Use maps and search results to locate records. Use the current source to establish what is true.

1. Resolve a known record ID through the maintained source map before broad search. Treat the map, cached summary, and index as pointers, not authoritative content.
2. Read the source as the task user through an authorized path. Record its stable ID, owner, revision or date, status, scope, and relevant exceptions.
3. Read implementation or system state separately when the question compares intent with behavior. Report both when they differ.
4. Check that citations resolve to the exact source and support the claim. Refresh results when revisions, permissions, or live state might have changed.
5. If sources conflict, access is unclear, or the authoritative record is unavailable, state the conflict and stop consequential action until the owner resolves it.
6. Keep indexes and handoffs to the minimum data needed. Do not copy protected content into a map or send private records to an unapproved index, embedding service, or external tool.
7. For retrieval systems, test known-ID lookup, stale-result detection, denied access, and permission revocation. Metadata fields alone do not enforce access control.
