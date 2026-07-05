# Marc MCP Assistant

Language: [中文](README.zh-CN.md) | **English** | [日本語](README.ja.md)

Marc MCP Assistant is a Windows-first, closed-source workflow assistant for
MSC Marc/Mentat users who want to connect Codex or other AI agents to a
controlled local Marc workflow.

It is not an official MSC/Hexagon product. It does not include Marc/Mentat, does
not provide Marc/Mentat licenses, and does not replace engineering judgment.

## Current Private Package

The current private trial line is:

```text
MarcMCP trial 2.5.0-trial
Platform: Windows
Delivery: private request only
Use with: local MSC Marc/Mentat + Codex MCP
```

GitHub Releases are not open yet. If your use case fits the current version, the
trial package and machine-bound trial license can be provided after contact.

## What It Can Help With

Many Marc users lose time not only on theory, but on repeated and fragile
workflow details:

- connect Codex to a local Marc/Mentat workflow through a controlled MCP server;
- check whether the local Marc/Mentat environment is visible to the assistant;
- confirm that Codex is using the delivered closed package, not an old or wrong path;
- organize model-inspection clues such as sets, links, boundaries, loads, and materials;
- collect solver-failure clues from logs, input files, and exit numbers;
- assist selected `.t16` result extraction and summary workflows;
- keep a clearer evidence trail for thesis, research, and engineering projects;
- provide a structured feedback path when you need support or diagnosis.

The goal is to make these local workflows more traceable, repeatable, and easier
to discuss with AI assistance.

## Typical Pain Points

You may want to try it if you often think:

- "I want Codex to help with Marc, but I need a controlled local connection."
- "I keep checking the same Mentat model details again and again."
- "Solver failure clues are scattered across logs and input files."
- "I need a cleaner record of what was checked, changed, and extracted."
- "I want post-processing and diagnosis to be less manual."

## Who It Is For

This may be useful if you are:

- using MSC Marc/Mentat for research, thesis work, or engineering projects;
- repeatedly checking model sets, links, boundaries, loads, or material setup;
- debugging solver failures, exit numbers, or convergence issues;
- exploring Codex-assisted Marc workflows;
- trying to organize post-processing and diagnostic evidence more clearly.

## Private Trial

Trial access is manual. If your use case fits the current version, you may
receive:

- a Windows closed-source trial package;
- a machine-bound trial license file;
- short installation and Codex configuration instructions;
- a feedback template for trial issues.

The trial may be limited by duration, machine, feature set, package version, or
support scope. It is intended to verify whether the tool helps your real Marc
workflow, not to provide an unlimited public version.

## Apply For Trial

Contact:

- Email: `1309224565@qq.com`
- WeChat: `18169419809`

When adding WeChat, please write:

```text
Marc MCP Trial
```

Please include:

```text
Marc/Mentat version:
Windows version:
Research or engineering field:
Current problem:
Solver exit number, if any:
Whether screenshots or log excerpts are available:
Need: trial / one-time diagnosis / monthly use / project support
```

Please do not send full model files at the first contact. Screenshots, short log
excerpts, and anonymized problem descriptions are enough for the first review.

## After You Receive The Package

Once you receive the private package and license, you can ask Codex to help with
setup using this guide:

- [Codex setup prompt](docs/codex-setup-prompt.md)
- [Trial installation](docs/trial-install.md)

The typical flow is:

```text
Receive package -> unzip locally -> run status check -> send machine code
-> receive license.json -> place license.json next to the executable under licenses
-> configure Codex MCP -> verify check_mcp_process_env -> start trial
```

## Important Boundaries

This project does not promise:

- automatic model correctness;
- guaranteed convergence;
- replacement of Marc/Mentat official software;
- replacement of Marc/Mentat licensing;
- unlimited free use;
- public access to core source code.

Model safety, engineering assumptions, and final conclusions remain the user's
responsibility.

## Documentation

- [Apply for trial](docs/apply.md)
- [Codex setup prompt](docs/codex-setup-prompt.md)
- [Trial installation](docs/trial-install.md)
- [Closed package notes](docs/trial-package.md)
- [FAQ](docs/faq.md)
- [Privacy](docs/privacy.md)
- [Contact](docs/contact.md)
- [Pain points](docs/pain-points.zh-CN.md)
- [Demo plan](docs/demo-plan.md)

## English Summary

Marc MCP Assistant is a Windows-first closed-source assistant for controlled
AI-assisted MSC Marc/Mentat workflows. Trial access is manual and license-bound.
Please contact the author with your Marc version, Windows version, field, and
current problem.
