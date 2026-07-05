# Trial Installation

This public document explains the expected private trial flow. The actual
package may include more specific instructions.

There is no public GitHub Release at this stage. First contact the author, then
use this page after you receive the private Windows package.

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

## What To Send Back For License

After the status check, send only the machine code and basic context requested by
the author. Do not send full model files at this stage.

Useful context:

- Marc/Mentat version;
- Windows version;
- research or engineering field;
- current problem;
- solver exit number, if any;
- whether you are applying for trial, diagnosis, monthly use, or project
  support.

## Codex Configuration

After receiving the package and license, use:

- [Codex setup prompt](codex-setup-prompt.md)

The most important verification is that `check_mcp_process_env` reports the
trial executable from the folder you just extracted.

If Codex reports another executable path, old package path, or developer source
directory, stop and fix the MCP configuration before running any Marc workflow.

## Current Distribution

At the current private beta stage, the Windows package is provided by request.
There is no public GitHub Release yet.

If public GitHub Releases are enabled later, users will still need to contact the
author for a trial or paid license.

## Safe Testing Advice

- Use backup, example, or non-critical models first.
- Keep your original Marc/Mentat model files unchanged until the workflow is
  verified.
- Read the command output carefully before allowing any workflow that writes
  files.
- Do not upload confidential models or license files unless there is an explicit
  support agreement.

## Feedback

If installation or authorization fails, please provide:

- Windows version;
- Marc/Mentat version;
- unzip folder path, if not sensitive;
- status check screenshot or text;
- license check screenshot or text;
- exact error message.

Please do not send full model files at the beginning.
