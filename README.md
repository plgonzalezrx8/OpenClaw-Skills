# ClawdBot Skills

A collection of custom skills for ClawdBot, extending its capabilities with specialized commands and integrations.

> **Note:** Each skill is published individually on [ClawdHub](https://clawdhub.com) for easy installation and use. This repository is the development home for collaboration, contributions, and skill improvements.

## What are ClawdBot Skills?

ClawdBot skills are modular extensions that add new capabilities to ClawdBot through shell scripts and command-line tools. Each skill is self-contained with its own documentation and dependencies.

## Available Skills

### Apple Remind Me
**Platform:** macOS only
**Description:** Natural language reminders that create actual Apple Reminders.app entries

Create, manage, and organize Apple Reminders using natural language. Works natively with Reminders.app and syncs across all your Apple devices (iPhone, iPad, Apple Watch).

**Features:**
- Create reminders with natural language time parsing
- List all incomplete reminders
- Complete reminders
- Edit reminder messages and times
- Delete reminders
- Native macOS integration with iCloud sync

**Documentation:** [apple-remind-me/SKILL.md](apple-remind-me/SKILL.md)

## Installation

1. Clone this repository:
```bash
git clone https://github.com/plgonzalezrx8/ClawdBot-Skills.git
```

2. Each skill may have its own requirements. Check the individual skill's `SKILL.md` file for:
   - Platform requirements (macOS, Linux, Windows)
   - Dependencies and binaries needed
   - Installation instructions

## Usage

Skills are organized in individual directories. Each skill contains:
- `SKILL.md` - Complete documentation for the skill
- Shell scripts or executables
- `.claude/` directory with ClawdBot configuration

To use a skill with ClawdBot, refer to the specific skill's documentation for available commands and examples.

## Skill Structure

Each skill follows this structure:
```
skill-name/
├── SKILL.md              # Complete documentation
├── .claude/              # ClawdBot configuration
├── *.sh                  # Shell scripts implementing functionality
└── [other files]         # Additional resources
```

The `SKILL.md` file includes:
- Skill metadata (name, description, platform requirements)
- Quick reference guide
- Detailed command documentation
- Usage examples
- Agent implementation guides

## Contributing

We welcome contributions! Whether you're fixing bugs, improving documentation, or adding new skills, your help is appreciated.

### How to Contribute

1. **Fork the repository** and create your branch from `master`
2. **Create a new directory** for your skill (if adding one)
3. **Add a `SKILL.md` file** with proper metadata and documentation
4. **Implement your functionality** in shell scripts or executables
5. **Test thoroughly** on the target platform(s)
6. **Submit a pull request** with a clear description of your changes

### Pull Request Guidelines

- Keep PRs focused on a single change
- Update documentation if you change functionality
- Ensure scripts are executable and include proper shebangs
- Test on all platforms your skill claims to support
- Follow existing code style and naming conventions

### Reporting Issues

- Use the issue tracker for bugs and feature requests
- Include your OS, ClawdBot version, and steps to reproduce
- Check existing issues before creating a new one

### Skill Metadata Format

Each `SKILL.md` should start with frontmatter:
```yaml
---
name: skill-name
description: Brief description of what the skill does
metadata: {"clawdbot":{"emoji":"🎯","os":["darwin","linux"],"requires":{"bins":["required-command"]}}}
---
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Support

For issues or questions:
- Check the individual skill's documentation
- Open an issue in this repository
- Refer to ClawdBot documentation

## Roadmap

- [ ] Add more cross-platform skills
- [ ] Linux-specific utilities
- [ ] Windows compatibility for existing skills
- [ ] Integration with popular APIs and services
