# person-eval

Claude Code skill for generating professional evaluations from Discourse forum
activity, inspired by Graham Duncan's "What's going on here, with this human?"
framework.

## Requirements

- Claude Code CLI
- discourse-mcp server configured (for accessing Discourse data)

## Installation

```bash
claude plugin marketplace add ducks/person-eval
claude plugin install person-eval@person-eval --scope user
```

## Usage

In a Claude Code session:

```
/person-eval ducks https://meta.discourse.org
```

Or with natural language:

```
evaluate sam on https://meta.discourse.org
```

The skill will:
1. Gather user profile and recent posts via discourse-mcp
2. Analyze communication patterns, expertise, and collaboration style
3. Generate a structured evaluation report

## Output

The evaluation includes:
- Executive summary
- Core strengths with evidence
- Growth areas
- Communication profile
- Collaboration dynamics
- Areas of expertise
- Representative quotes
- Discussion prompts for 1:1s

## License

MIT
