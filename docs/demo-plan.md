# Public Demo Plan

Public demo media should show value without exposing implementation or private
customer data.

## Demo Topics

1. Package starts in locked mode and shows contact path.
2. Licensed package passes `status` and `package-check`.
3. Codex connects to the guarded MCP server.
4. Marc environment check returns structured evidence.
5. A sanitized demo workflow creates or inspects a simple model.
6. A sanitized post-processing example extracts a result curve.

## Do Not Show

- private signing keys;
- customer license files;
- package source files;
- customer models;
- real project paths;
- license server addresses;
- paid package download links;
- internal strategy documents.

## Safe Visuals

- simple synthetic model;
- cropped terminal output with paths blurred;
- generated demo `.t16` or official tutorial-style example only if allowed;
- public README and trial application page;
- before/after workflow diagram.

## Minimum Demo Script

```text
1. Explain Marc user pain point.
2. Show package-check passes.
3. Show Codex sees Marc MCP tools.
4. Run one safe demo command.
5. Show generated evidence/result.
6. End with trial application contact.
```
