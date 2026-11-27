# Exepal agent skills

Free agent skills from [Exepal](https://exepal.com). They follow the open `SKILL.md` format, so they work in
OpenClaw, Claude Code, Codex and other agents that load skills.

## check-skill-before-install

Makes your agent scan any skill it is about to install with [Skill Check](https://exepal.com/skill-check),
and refuse the ones that carry malware set-up steps, credential theft or hidden instructions.

- Works on ClawHub links, GitHub skill folders, a raw `SKILL.md` URL, or pasted text.
- Shows the file, the line and why each finding matters.
- 20 free checks a day, no sign-up. Then $0.005 a skill with a free key.

### Install

Claude Code:

```bash
mkdir -p ~/.claude/skills && cp -r skills/check-skill-before-install ~/.claude/skills/
```

Codex: copy the folder into `~/.codex/skills/`. OpenClaw: copy it into your workspace `skills/` folder.

Or use it as a tool instead: add the MCP server `https://api.exepal.com/mcp` and call `skill_check`.

### Try it without installing anything

Paste a link at **https://exepal.com/skill-check** (3 free checks a day in the browser).

## License

MIT
