# Learning Partner

An AI skill that reshapes coding assistant responses to support **developer learning** instead of cognitive offloading. It guides you through understanding before solutions, explains reasoning alongside code, and uses Socratic debugging.

Research shows developers who offload thinking to AI score 17% lower on skill mastery. This skill ensures you grow your skills while still benefiting from AI speed.

## What It Does

- **Understand-first, code-second** — explains "why" before "what"
- **Guided debugging** — asks for your hypothesis before revealing fixes
- **Progressive disclosure** — concept → structure → implementation
- **Escape hatch** — say "just do it" or "skip teaching" when you're in a rush

## Installation

### Warp / Agents

Clone this repo into your `~/.agents/skills/` directory:

```sh
mkdir -p ~/.agents/skills
git clone https://github.com/dani-fadli/learning-partner.git ~/.agents/skills/learning-partner
```

The skill will be automatically picked up by Warp's Oz agent on your next session.

### Cursor

Clone into your `~/.cursor/skills/` directory:

```sh
mkdir -p ~/.cursor/skills
git clone https://github.com/dani-fadli/learning-partner.git ~/.cursor/skills/learning-partner
```

### Manual Installation

1. Copy `SKILL.md` (and the `references/` folder) into your agent's skill directory.
2. The exact path depends on your tool — common locations:
   - `~/.agents/skills/learning-partner/`
   - `~/.cursor/skills/learning-partner/`

## Usage

Once installed, the skill activates automatically on every coding prompt. No special commands needed — just ask for help with code, debugging, features, refactoring, or architecture as you normally would.

### Override / Direct Mode

When you're in a hurry, use any of these phrases to skip the teaching flow:

- "just do it" / "just give me the code"
- "skip teaching" / "no explanation needed"
- "I'm in a rush" / "deadline mode" / "ship it"

## Structure

```
learning-partner/
├── SKILL.md                          # Main skill definition
├── references/
│   └── interaction-patterns.md       # Research backing the approach
└── README.md
```

## License

MIT
