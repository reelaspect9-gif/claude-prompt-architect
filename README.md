# Prompt Architect for Claude Code

Prompt Architect supports your existing Prompt Engineer. The engineer processes the initial raw request first; Architect then receives the raw request, engineered prompt, and active project rules to develop an EXECUTION BRIEF. It deepens production dependencies, asset specifications, acceptance evidence, and handoffs without replacing the engineer or rewriting its work unnecessarily.

Repository: [reelaspect9-gif/claude-prompt-architect](https://github.com/reelaspect9-gif/claude-prompt-architect)

## Set up the subagent

Download the [raw agent definition](https://raw.githubusercontent.com/reelaspect9-gif/claude-prompt-architect/main/.claude/agents/prompt-architect.md), preserving its Markdown contents and YAML frontmatter. Save a copy at one of these documented Claude Code locations:

- One project: `<your-project>/.claude/agents/prompt-architect.md`
- All your projects: `~/.claude/agents/prompt-architect.md`

Create the parent directories if needed. The `~` location refers to your user home directory. Keep the filename ending in `.md`; do not save a GitHub preview page as the agent file. In GitHub, use the file's raw content or download option.

Check whether a same-name definition already exists before saving. Preserve existing content and customizations. Do not overwrite or replace that definition without explicit permission; prepare the proposed additions separately for review. Avoid installing competing copies unless you deliberately understand their scope and precedence.

The file uses the [official custom-subagent format](https://code.claude.com/docs/en/sub-agents): `name` and `description` in YAML frontmatter, followed by the instructions. It does not prescribe a model, tool list, hooks, or credentials. Available capabilities depend on your Claude Code environment. If a newly added agent is not discovered, verify its location and start a fresh Claude Code session.

## Use the pair before production

Ask the lead Claude session to delegate explicitly:

> First use my existing Prompt Engineer to interpret and structure this request. Then use prompt-architect as its supporting production architect. Pass both versions and the active master rules. Preserve the sources, deepen the implementation gaps, and resolve any change proposals with the engineer. Return the reconciled EXECUTION BRIEF to the lead for Quality Director review before dependent production begins.

Supply the relevant rules and references with your request. For example:

> I want a premium custom shop interior with convincing materials, readable signs, and smooth character interactions. Keep the established illustrated characters. Expand this into an actionable brief without inventing the period, exact dimensions, or extra story events.

For ongoing work, the pair amends affected prompt and brief versions while preserving accepted work. A change to one prop should not restart production. Architect returns a derivation summary of at most 100 words alongside the detailed brief.

Installing this file does not intercept prompts, automatically enforce the sequence, or create a `/prompt-architect` slash command. The lead must actually invoke the existing engineer and delegate to Architect. Add this sequence to your existing project instructions if desired, preserving their other rules. No automatic hooks are included.

## Existing Prompt Engineer compatibility

The [AI Templates Prompt Engineer candidate](https://github.com/davila7/claude-code-templates/blob/main/cli-tool/components/agents/ai-specialists/prompt-engineer.md) focuses on prompt text and structure for a selected model; Architect adds production decomposition and execution specifications. This public reference does not prove which version or component you installed. At runtime, inspect the actual active definition and interface. A same-name skill and subagent are not interchangeable. Preserve the existing component and its customizations; this repository does not install or replace it.

## Scope and limits

The agent can specify blueprint analysis, original modeling and texture work, genuine 4K requirements where applicable, animated material states, character inheritance, motion and contact, typography, audio, and practical proof gates. It scales these sections to the actual request. “Smooth” does not automatically mean higher frame rate or more blur; “complex” does not mean unnecessary parts.

The brief is not a completed production asset or a quality guarantee. Quality Director and other roles must correspond to actual delegated reviewers or explicitly identified alternatives. This repository does not install additional agents, fonts, rendering software, or external services.

The definition has been checked as a written configuration. It has not been live-tested in Claude Code or validated through a finished production. Review the pair's first brief for intent fidelity before dependent work.
