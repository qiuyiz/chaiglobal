# Install Selah

Unzip this file, then ask Claude Code to read this file:

```
Hey Claude, read INSTALL.md and follow the instructions.
```

That's it. Claude will do the rest.

---

## Instructions for Claude

Install the Selah contemplative development framework:

1. **IMPORTANT: Do NOT overwrite the user's existing CLAUDE.md.** If the project already has a CLAUDE.md, append the contents of the Selah `CLAUDE.md` to the end of their existing file. If no CLAUDE.md exists, copy it as-is to the project root.
2. Create the directory `~/.claude/commands/` if it doesn't exist.
3. Copy `.claude/commands/selah.md` to `~/.claude/commands/selah.md` (this makes `/selah` available globally in all projects).

After installing, tell the user:

- **Selah is installed.** The redemptive framework is now in your project's CLAUDE.md.
- **`/selah`** is available globally — type it anytime for a contemplative pause connected to your current work.
- To add Selah to another project, append the Selah section from `CLAUDE.md` into that project's CLAUDE.md.
