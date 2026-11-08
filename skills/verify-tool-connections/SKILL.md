---
name: verify-tool-connections
description: Verify a new MCP server or connected tool's permissions, discovery, and real behavior. Use when a connection appears configured but its actual access or output is not yet proven.
license: Apache-2.0
---

# Verify tool connections

A saved connection is not proof that a tool is available or working.

1. Check the host's current setup guide and version. Confirm the server, account, authentication method, requested scopes, and tools it exposes.
2. Inspect which tools read data and which can write or trigger external actions. Check where prompts and returned data travel. Resolve unclear access or data handling before sending sensitive input.
3. Start with the narrowest suitable scope and an authorized read against non-sensitive or approved data. Do not use a write action as a connectivity test.
4. Record each state separately: configured, connected, discovered, executed, and output verified. A missing state is not a pass.
5. Inspect the actual tool call and returned source. Open the cited destination or record and confirm the result supports the task. Mark a normal answer with no tool call as not executed.
6. Diagnose one failure using current host and server evidence. Do not invent tool output or claim setup success from configuration alone.
7. Remove a connection only when it was temporary or the user asked for removal. Preserve persistent settings unless the user authorized a change.
