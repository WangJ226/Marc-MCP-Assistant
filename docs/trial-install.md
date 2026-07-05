# Trial Installation

This public document explains the expected flow. The actual package may include
more specific instructions.

## Requirements

- Windows.
- Local MSC Marc/Mentat already installed.
- Valid Marc/Mentat license from your own organization or vendor.
- Marc/Mentat can start normally without this assistant.
- Backups of any model files before testing.

## Basic Flow

```text
Receive private package
-> unzip to a local folder
-> run status check
-> send machine code to the author
-> receive license.json
-> put license.json in the licenses folder next to the exe
-> configure Codex MCP
-> verify the MCP process path
-> test limited workflows on backup or non-critical models
```

The expected license location is:

```text
<folder-containing-the-exe>\licenses\license.json
```

If the zip extracts into nested folders, use the folder that actually contains
the `.exe`.

## Codex Configuration

After receiving the package and license, use:

- [Codex setup prompt](codex-setup-prompt.md)

The most important verification is that `check_mcp_process_env` reports the
trial executable from the folder you just extracted.

## Current Distribution

At the current private beta stage, the Windows package is provided by request.
There is no public GitHub Release yet.

If public GitHub Releases are enabled later, users will still need to contact the
author for a trial or paid license.

## Feedback

If installation or authorization fails, please provide:

- Windows version;
- Marc/Mentat version;
- unzip folder path, if not sensitive;
- status check screenshot or text;
- license check screenshot or text;
- exact error message.

Please do not send full model files at the beginning.
