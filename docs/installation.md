# Installation and compatibility

## Requirements

- An AI assistant or agent that supports loading skills compatible with the `SKILL.md` format.
- A purchased copy of the **StoryForge Pro** ZIP.
- No Jira or Confluence account is needed for text-only output.

## Installation steps

1. Download the purchased ZIP from the authorized marketplace.
2. Extract it to a local directory. Verify `SKILL.md` is present alongside its `references`, `templates`, and `examples` folders.
3. Use your agent's official skill installation/import feature, or the agent-specific skills directory described in its documentation. Do not place a ZIP in an arbitrary plugin folder unless your agent specifically supports that.
4. Start a new agent session if needed, then ask: `Use StoryForge Pro to create a Jira-ready story from this idea: [your idea]`.
5. Confirm the assistant asks clarification questions as needed and flags unconfirmed business decisions.

> Installation screens and paths differ across Claude Code, Codex CLI, Cursor, VS Code Copilot, Gemini CLI, and other hosts. Support for SKILL.md does not imply support for every optional integration. Refer to the current documentation for your specific agent.

## Optional Jira / Confluence integration

The skill has no built-in direct Jira API authentication. If your agent is connected to Jira or Confluence through an approved integration, you can ask it to look up relevant material or prepare a change. Check the connected tool's permissions. **Always review and approve the preview before writing issues or pages.**

## Troubleshooting

If your agent does not recognize StoryForge Pro, verify that it supports custom skills, that `SKILL.md` was extracted and registered correctly, and that the complete directory structure was preserved. If the host lacks skill support, use a compatible agent.
