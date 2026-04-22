# Agentic Coding with Claude Code

Code repository for [Agentic Coding with Claude Code, First Edition](https://www.packtpub.com/en-us/product/agentic-coding-with-claude-code-first-edition/9781806022595) by Eden Marco.

---

## Using Claude on GitHub

This repo has Claude Code integrated via GitHub Actions.

### Trigger Claude in any PR or issue

Mention `@claude` in a comment:

```
@claude fix the failing test in src/foo.ts
@claude review this PR
@claude add input validation to the form
@claude explain what this function does
```

Claude reads the full context (code, diffs, conversation history) and responds or implements changes directly.

### Automatic PR reviews

Every new or updated PR gets an automatic code review — no `@claude` mention needed.

### Workflows

| File | Trigger | Purpose |
|------|---------|---------|
| `.github/workflows/claude.yml` | `@claude` mention | Interactive assistant |
| `.github/workflows/claude-code-review.yml` | PR open/update | Automatic code review |

### Expand allowed tools

By default Claude can read/write files and interact with the repo (comments, branches, commits). Add more in the workflow file:

```yaml
allowed_tools: Bash(npm install),Bash(npm run build),Bash(npm run test)
```

---

## Chapters

1. Context Engineering
2. The GIST of Claude Code
3. Getting Started with Claude Code – A Tour of Essential Commands
4. Extending Claude Code with MCP Servers and Plugins
5. Automating Your Development Workflow with Claude Code and GitHub
6. Claude Code Planning and Multi-Agent Workflows
7. Working with Claude Code Subagents
8. Creating and Customizing Output Styles
9. Understanding Agent Skills
10. Using Claude Code Desktop
11. Understanding Deep Agents
