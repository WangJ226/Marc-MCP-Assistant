# Codex Setup Prompt

After you receive the private Windows package and `license.json`, you can ask
Codex to help you configure the local MCP connection.

Copy this prompt into a new Codex chat. Replace the paths with your own package
folder.

```text
I have received a private Marc MCP Assistant Windows trial package.

Please help me configure it as a local Codex MCP server.

Important rules:
1. Do not search for or use any developer source directory.
2. Only use the package folder I provide below.
3. Do not upload or modify my Marc model files.
4. First verify the executable path and license placement.

Package folder:
<paste-the-folder-that-contains-the-exe-here>

Expected license path:
<folder-containing-the-exe>\licenses\license.json

Please:
1. Find the MarcMCP trial executable in this folder.
2. Confirm that license.json is placed under the licenses folder next to the exe.
3. Run the package status or package-check command if available.
4. Show me the local Codex MCP setup steps for an MCP server named marc-control.
5. After I add the config and restart Codex, call check_mcp_process_env.
6. Confirm that sys_executable points to this trial exe, not another internal or old path.
7. Then run a basic Marc/Mentat environment check.
```

## Expected Codex MCP Setup Shape

The exact executable name may differ by version. In general, the local MCP
server should be named `marc-control`, the command should point to the trial
executable, and the arguments should start the `mcp-server` mode with your
preferred language.

Use `zh-CN` for Chinese messages, `en` for English messages, or `ja` for
Japanese messages if needed.

## What To Verify

After configuration, ask Codex to call:

```text
check_mcp_process_env
```

The returned `sys_executable` should point to the executable in the private
package folder you received.

If it points to another folder, old package, or developer path, stop and fix the
Codex MCP config before running Marc workflows.
