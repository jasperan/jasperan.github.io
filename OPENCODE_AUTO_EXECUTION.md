# OpenCode Auto-Execution Configuration

**Modified:** March 3, 2026  
**Purpose:** Enable automatic execution of all tools and commands without supervision

---

## Changes Made

### Permission Configuration

Updated `~/.config/opencode/opencode.json` to automatically allow all tools:

**Before:**
```json
"permission": {
  "edit": "allow",
  "bash": "allow",
  "webfetch": "allow",
  "websearch": "allow",
  "mcp_context7*": "allow",
  "mcp_playwright*": "allow",
  "mcp_serena*": "allow"
}
```

**After:**
```json
"permission": {
  "read": "allow",
  "write": "allow",
  "edit": "allow",
  "bash": "allow",
  "glob": "allow",
  "grep": "allow",
  "webfetch": "allow",
  "websearch": "allow",
  "skill": "allow",
  "task": "allow",
  "question": "allow",
  "context7_resolve-library-id": "allow",
  "context7_query-docs": "allow",
  "mcp_*": "allow"
}
```

---

## What This Means

### ✅ Automatic Execution

OpenCode will now execute all operations **without asking for confirmation**:

- **File Operations:** Read, write, edit files automatically
- **Terminal Commands:** Run bash commands without approval
- **Search Tools:** Glob and grep operations auto-approved
- **Web Tools:** Fetch URLs and search the web automatically
- **Skills:** Invoke and use all skills without prompting
- **Tasks:** Spawn subagents automatically
- **Questions:** Ask clarifying questions without supervision
- **MCP Tools:** All Model Context Protocol tools auto-approved

### ⚠️ Safety Considerations

**This is similar to `--dangerously-skip-permissions` in Claude Code:**

- ⚠️ **No confirmation prompts** for any operations
- ⚠️ **Files can be modified or deleted** without approval
- ⚠️ **Commands run without review** (including potentially destructive ones)
- ⚠️ **Web requests made automatically**

**Only use this configuration if you:**
- Trust the AI's judgment completely
- Understand the risks of automatic execution
- Have backups of important data
- Are working in a safe, isolated environment

---

## Backup & Revert

### Backup Created

Original configuration backed up to:
```
~/.config/opencode/opencode.json.backup
~/.config/opencode/opencode.json.auto-approved
```

### How to Revert

To restore the original (safer) configuration:

```bash
cd ~/.config/opencode
cp opencode.json.backup opencode.json
# Restart OpenCode
```

Or manually edit `~/.config/opencode/opencode.json` and remove the `"allow"` permissions you don't want.

---

## Alternative: Selective Permissions

If you want automatic execution for some tools but not others, you can mix permissions:

```json
"permission": {
  "read": "allow",           // Always allow reading
  "write": "ask",            // Ask before writing
  "edit": "ask",             // Ask before editing
  "bash": "ask",             // Ask before bash commands
  "glob": "allow",           // Always allow glob
  "grep": "allow",           // Always allow grep
  "webfetch": "allow",       // Always allow web fetch
  "websearch": "allow",      // Always allow web search
  "skill": "allow",          // Always allow skills
  "task": "ask",             // Ask before spawning tasks
  "question": "allow",       // Always allow questions
  "mcp_*": "allow"           // Allow all MCP tools
}
```

### Permission Values

- `"allow"` - Always execute automatically (no prompts)
- `"ask"` - Ask for confirmation before each operation
- `"deny"` - Never allow the operation

---

## Verification

To verify the configuration is working:

1. **Restart OpenCode** (if currently running)
2. Try a file operation: "Create a test file called test.txt"
3. Try a bash command: "List files in current directory"
4. Both should execute **without** asking for permission

---

## Troubleshooting

### If OpenCode Still Asks for Permission

1. **Check JSON validity:**
   ```bash
   cat ~/.config/opencode/opencode.json | jq .
   ```

2. **Verify permissions section:**
   ```bash
   cat ~/.config/opencode/opencode.json | jq '.permission'
   ```

3. **Restart OpenCode completely** (not just the current session)

4. **Check for typos** in tool names

### If OpenCode Won't Start

1. **Restore backup:**
   ```bash
   cd ~/.config/opencode
   cp opencode.json.backup opencode.json
   ```

2. **Validate JSON:**
   ```bash
   jq . opencode.json
   ```

---

## Comparison with Claude Code

| Feature | Claude Code | OpenCode |
|---------|-------------|----------|
| **Flag** | `--dangerously-skip-permissions` | Config file setting |
| **Location** | Command-line argument | `~/.config/opencode/opencode.json` |
| **Granularity** | All or nothing | Per-tool configuration |
| **Persistence** | Per session | Permanent (until changed) |
| **Safety** | Explicit opt-in | Config file modification |

---

## Security Best Practices

When using auto-execution:

1. **✅ DO:**
   - Use in development/sandbox environments
   - Keep backups of important files
   - Review the AI's actions periodically
   - Use version control (git) for important projects

2. **❌ DON'T:**
   - Use in production environments
   - Run with access to critical system files
   - Leave unattended in sensitive directories
   - Share the config file with API keys

---

## Files Modified

- `~/.config/opencode/opencode.json` - Updated permissions
- `~/.config/opencode/opencode.json.backup` - Original backup (pre-existing)
- `~/.config/opencode/opencode.json.auto-approved` - Backup of auto-approved config

---

**Configuration active immediately. Restart OpenCode if currently running.**
