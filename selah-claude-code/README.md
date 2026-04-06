# Selah for Claude Code

**Contemplative AI development tools from CHAI Global × FaithTech.**

Selah embeds FaithTech's [Redemptive Technology](https://faithtech.com/playbook) framework directly into your Claude Code workflow. It's two files you drop into any project — no installation, no dependencies, no configuration.

## What It Does

**CLAUDE.md** gives Claude Code a redemptive operating posture. Instead of optimizing purely for speed, Claude operates as a co-creator — asking better questions before jumping to solutions, applying the 3RC discernment framework (Reject/Receive/Reimagine/Create) before suggesting new technology, and defaulting to simplicity over complexity.

**/selah** is a breath prayer command. Type `/selah` at any point during a coding session, and Claude surfaces a contemplative prayer matched to your current context (starting work, debugging, post-completion, after a setback). Then it pauses. No suggestions, no next steps — just stillness. You resume when you're ready.

## Quick Start

### Option A: Add to an existing project

Copy the two items into your project root:

```bash
# From this repo, copy into your project:
cp CLAUDE.md /path/to/your/project/CLAUDE.md
cp -r .claude /path/to/your/project/.claude
```

That's it. Next time you run `claude` in that project directory, Claude Code loads the CLAUDE.md context and the /selah command automatically.

### Option B: Clone and use as a template

```bash
git clone https://github.com/chai-global/selah-claude-code.git
cd selah-claude-code

# Start Claude Code — it picks up CLAUDE.md automatically
claude
```

### Option C: Add to your global Claude Code config

If you want Selah active in *every* project, not just specific ones:

```bash
# Copy the command to your global commands directory
mkdir -p ~/.claude/commands
cp .claude/commands/selah.md ~/.claude/commands/selah.md
```

For the CLAUDE.md context to apply globally, add its contents to your Claude Code settings under the system prompt / project instructions. (Note: project-level CLAUDE.md files override global settings, so if a project has its own CLAUDE.md, you'll need to include the Selah content there too.)

## Usage

### Working with CLAUDE.md

Once CLAUDE.md is in your project root, Claude Code automatically reads it at the start of every session. You don't need to do anything — the redemptive framework shapes Claude's behavior silently.

You'll notice Claude:

- **Asks more questions before coding.** Especially at the start of a new feature. It wants to understand who's affected by the problem before jumping to implementation.
- **Applies 3RC at decision points.** When you ask Claude to add a dependency, build a new service, or introduce a feature, it briefly considers: Should we reject this (is tech the answer?), receive an existing solution, reimagine something that exists, or create something new?
- **Defaults to simplicity.** Claude will sometimes push back on complexity and ask "what can we remove?" This isn't obstruction — it's the kenotic design principle from the Playbook.
- **Doesn't preach.** The framework operates in the background. Claude won't quote Scripture at you or moralize about your architectural decisions unless you've explicitly set that context.

### Evaluating your project

Ask Claude to evaluate your project against the FaithTech framework at any time:

```
> Evaluate this project using the 3RC framework.
```

Claude will walk through each posture (Reject, Receive, Reimagine, Create) and assess where your project sits on the Reckless → Responsible → Redemptive spectrum. It's honest, specific, and constructive.

You can also ask more targeted questions:

```
> Where does this feature fall on the Reckless/Responsible/Redemptive spectrum?
> Apply 3RC to this proposed architecture.
> Who are the image-bearers affected by this design decision?
> What would "redemptive" look like for this user flow?
```

### Using /selah

Type `/selah` in Claude Code at any point. Claude will:

1. Select a breath prayer that fits your current work context
2. Present the inhale/exhale phrases with a Scripture reference
3. Wait silently for you to resume

There's no timer enforcing the 90-second suggestion — it's an invitation, not a constraint. Take 30 seconds or 10 minutes. Claude doesn't follow up, check on you, or suggest next steps. It waits.

**When to use it:**
- Before starting a deep coding session
- After a frustrating debugging stretch
- When you've just shipped something
- At any natural transition point
- When you feel the pull to rush past something important
- Whenever you want to

## File Structure

```
your-project/
├── CLAUDE.md                    # Redemptive framework context (Claude reads this automatically)
├── .claude/
│   └── commands/
│       └── selah.md             # Breath prayer command
├── ... (your project files)
```

## Customizing the Prayer Library

The prayer library lives in `.claude/commands/selah.md`. It's organized by context:

- **Starting new work** — prayers about guidance and creation
- **Debugging / stuck** — prayers about patience and wisdom
- **After completing something** — prayers of gratitude
- **After a setback** — prayers of comfort and perseverance
- **Transitioning between tasks** — prayers about direction
- **End of session** — prayers of rest and peace

To add your own prayers, edit the file directly. Follow the format:

```
- Inhale: "first phrase" / Exhale: "second phrase" — Scripture Reference
```

We welcome contributions from the FaithTech and CHAI communities. Submit a pull request with prayers from your tradition, your church, or your own devotional life.

## How It Works (Technical)

**CLAUDE.md** is Claude Code's project configuration file. When you run `claude` in a directory containing a CLAUDE.md, Claude reads it as system-level context before any interaction. It shapes Claude's personality, priorities, and decision-making patterns for that session. No API calls, no external services — it's just a text file that Claude reads.

**Custom commands** in `.claude/commands/` are markdown files that define reusable prompts. The filename (minus `.md`) becomes the slash command name. When you type `/selah`, Claude Code reads `selah.md` and executes its instructions. Again — no external services, no dependencies. Just markdown.

This means:
- **Zero installation.** Copy two files. Done.
- **Zero dependencies.** No npm packages, no pip installs, no Docker containers.
- **Zero cost.** No API keys, no subscriptions, no cloud services.
- **Fully offline.** Everything runs locally in your Claude Code session.
- **Fully customizable.** Edit the markdown files however you want.

## Compatibility

- **Claude Code** — full support (CLAUDE.md + slash commands)
- **Cursor** — CLAUDE.md works as a rules file (rename to `.cursorrules` or add to Cursor settings). Slash commands are not supported in Cursor; use the prayer library content as a prompt instead.
- **Claude Desktop** — CLAUDE.md content can be added as a project instruction. Slash commands are not supported; copy the prayer library into your project knowledge.

## About

Selah is a collaboration between [CHAI Global](https://chai-global.org) (Christians in AI) and [FaithTech](https://faithtech.com). It implements FaithTech's [Redemptive Technology Playbook](https://faithtech.com/playbook) and [4D Cycle Workbook](https://workbook.faithtech.com) as practical developer tooling.

**"Selah"** appears 71 times in the Psalms — a liturgical instruction to pause, reflect, and listen before continuing. That's what this does for your development workflow.

### License

MIT — same as FaithTech's workbook. Use it, fork it, share it.
