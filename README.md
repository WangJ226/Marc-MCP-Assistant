# Marc MCP Assistant

Language: [中文](README.zh-CN.md) | **English** | [日本語](README.ja.md)

Marc MCP Assistant is a Windows-first, closed-source workflow assistant for MSC
Marc/Mentat users. It connects Codex or other AI agents to a controlled local
Marc workflow through MCP, so Marc-related checks, diagnosis clues, and selected
post-processing tasks can be handled in a more traceable way.

It is not an official MSC/Hexagon product. It does not include Marc/Mentat, does
not provide Marc/Mentat licenses, and does not replace engineering judgment.

## Current Version Status

```text
Current private trial line: MarcMCP trial 2.5.0-trial
Platform: Windows
Stage: private beta
Delivery: contact author first, then private package + trial license
Use with: local MSC Marc/Mentat + Codex MCP
Public GitHub Release: not open yet
```

The current version is already suitable for guided private trials. New features
are still under active development, and real Marc/Mentat user feedback is
welcome.

## Supported In The Current Version

The current closed package focuses on practical Marc workflow assistance:

- start a controlled local MCP server for Codex;
- check package status and license status;
- show the machine code needed for trial licensing;
- verify that Codex is using the delivered package path, not an old or wrong
  executable;
- check whether the local MSC Marc/Mentat environment can be detected;
- initialize a local Marc project workspace for assisted workflows;
- run basic MCP doctor/environment checks;
- help organize model-inspection clues such as sets, links, boundaries, loads,
  and materials;
- help collect solver-failure clues from logs, input files, and exit numbers;
- assist selected `.t16` result extraction and summary workflows;
- keep a clearer evidence trail for thesis, research, and engineering projects;
- provide a structured feedback path when support or diagnosis is needed.

## Problems It Is Designed To Reduce

Many Marc users lose time on repeated, fragile workflow details rather than on
the theory itself. This project is designed to reduce:

- repeated manual checking of Mentat model details;
- confusion about which executable or workflow Codex is actually using;
- scattered solver-failure evidence across logs, input files, and screenshots;
- manual post-processing records that are hard to reproduce later;
- unclear traces of what was checked, changed, extracted, and discussed;
- difficulty explaining Marc workflow problems to an AI assistant or support
  person.

The goal is not to make Marc automatic. The goal is to make local Marc workflows
more controlled, traceable, repeatable, and easier to discuss with AI assistance.

## In Active Development

Planned and ongoing work includes:

- broader Marc/Mentat workflow coverage;
- better solver-failure diagnosis templates;
- more post-processing helpers for common `.t16` workflows;
- clearer multilingual guidance in Chinese, English, and Japanese;
- improved trial, feedback, and support workflow;
- private-package updates based on real user problems.

If your field has special Marc/Mentat workflows, feedback is welcome. Real user
problems are the most useful input for deciding what to improve next.

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
AI-assisted MSC Marc/Mentat workflows. The current private package is
`MarcMCP trial 2.5.0-trial`. Trial access is manual and license-bound. Please
contact the author with your Marc version, Windows version, field, and current
problem.
