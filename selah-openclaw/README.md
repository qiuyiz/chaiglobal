# Selah for OpenClaw

A contemplative AI agent workspace built on redemptive technology principles from the **CHAI Global × FaithTech** partnership.

Selah transforms your OpenClaw agent into an unhurried co-creator — one that builds with wisdom, pauses for reflection, and keeps the people who will use your work at the center of every decision.

## What's Included

```
selah-openclaw/
├── SOUL.md              # Agent identity — redemptive posture, kenotic defaults
├── AGENTS.md            # Operating rules — 3RC discernment, 4D cycle, guardrails
├── HEARTBEAT.md         # Contemplative rhythm — auto-Selah, morning intentions, sabbath mode
├── USER.md              # Your profile — customize faith context, preferences, channels
├── skills/
│   └── selah/
│       └── SKILL.md     # Breath prayer skill — contextual Scripture + reflection
└── README.md            # This file
```

## Quick Start

### Option 1: Full Workspace (New Agent)

Copy this entire folder as your OpenClaw workspace:

```bash
cp -r selah-openclaw/ ~/.openclaw/agents/selah/
```

Edit `USER.md` with your name, projects, and preferences. Start the gateway.

### Option 2: Add to Existing Agent

Append the Selah identity to your existing SOUL.md:

```bash
cat selah-openclaw/SOUL.md >> ~/.openclaw/agents/my-agent/SOUL.md
```

Copy the operating rules and skill:

```bash
cat selah-openclaw/AGENTS.md >> ~/.openclaw/agents/my-agent/AGENTS.md
cp -r selah-openclaw/skills/selah ~/.openclaw/agents/my-agent/skills/
```

Merge the HEARTBEAT.md entries into your existing heartbeat file, or replace it if you don't have one.

### Option 3: Skill Only

If you just want the breath prayer without the full redemptive framework:

```bash
cp -r selah-openclaw/skills/selah ~/.openclaw/skills/
```

This makes the `selah` skill available to any agent. They can invoke it, but won't have the redemptive operating posture or auto-rhythm.

## How It Works

### The Selah Rhythm

Unlike a chatbot that forgets to pause, OpenClaw's heartbeat scheduler checks every 25 minutes whether a contemplative moment would serve you. If you've been deep in work, it offers a breath prayer — a short inhale/exhale phrase drawn from Scripture and connected to whatever you're actually building.

This is an invitation, not an interruption. Decline it and the agent moves on. Accept it and you get 90 seconds of stillness before resuming.

You can also trigger it manually anytime by asking for a Selah moment.

### 3RC Discernment

Before the agent suggests new tools, automations, or workflows, it runs through:

1. **Reject** — Is technology even the right answer here?
2. **Receive** — Does something already exist?
3. **Reimagine** — Can something existing be adapted?
4. **Create** — Only then, build something new.

### Sabbath Mode

Configure sabbath hours in `USER.md`. During those hours, the agent refuses non-emergency work and encourages rest. Override with "this is urgent" if needed.

### Morning Intentions

Enable in `USER.md` to receive a brief daily verse connected to your current projects. Three lines, no sermon.

## Customization

### Scripture Preferences

Edit `USER.md` to set your preferred Bible translation, comfort level with Scripture references, and prayer style.

### Rhythm Tuning

Adjust the heartbeat interval in `HEARTBEAT.md`. Default is 25 minutes (one Pomodoro). Set to "Only when I ask" in `USER.md` to disable auto-Selah entirely.

### Adding Your Own Prayers

The Builder's Library in `skills/selah/SKILL.md` is a starting point. Add verses that speak to your specific work — your industry, your community, the problems you're solving.

## The Framework

Selah is built on FaithTech's redemptive technology framework:

- **Three Ways of Technology**: Reckless → Responsible → Redemptive
- **3RC Discernment**: Reject, Receive, Reimagine, Create
- **4D Cycle**: Discover, Discern, Develop, Demonstrate
- **Kenotic Design**: Self-emptying as a design principle — do less, serve more

## Compatibility

- **OpenClaw**: Full support — SOUL.md, AGENTS.md, HEARTBEAT.md, skills
- **Claude Code**: See the companion `selah-claude-code` package (CLAUDE.md + `/selah` command)
- **Cursor / Windsurf**: Use SOUL.md as your rules file, manually invoke the selah skill
- **Claude Desktop / MCP**: Coming in Phase 3

## Credits

**CHAI Global × FaithTech Partnership**

A collaboration between CHAI Global and FaithTech, grounded in FaithTech's Redemptive Technology framework and the Builder's Catechism.

---

*"Unless the Lord builds the house, the builders labor in vain." — Psalm 127:1*
