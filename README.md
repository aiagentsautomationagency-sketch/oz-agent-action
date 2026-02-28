# Oz Skills

A curated collection of reusable [Agent Skills](https://agentskills.io) for Warp AI agents and Oz.

## What Are Agent Skills?

Agent Skills are markdown files that teach AI agents about your conventions, best practices, and workflows. When you work with agents in Warp, they automatically discover and use these skills to provide context-aware help.

Think of skills as onboarding guides that help agents understand how you work.

## How Skills Work

- **Skills live in `.agents/skills/` directories** - either in your project (`.agents/skills/`) or globally (`~/.agents/skills/`)
- **Each skill is a folder** containing a `SKILL.md` file with YAML frontmatter and markdown content
- **Warp agents automatically discover** and load skills when relevant to your current task

## Using These Skills

To use a skill from this repository:

1. Copy the skill folder (e.g., `docs-update`) from `.agents/skills/` 
2. Paste it into your project's `.agents/skills/` directory, or
3. Paste it into `~/.agents/skills/` to use it across all projects

Warp will automatically detect the new skill on your next interaction.

## Available Skills

- **[ci-fix](.agents/skills/ci-fix)** — Diagnose and fix GitHub Actions CI failures. Inspects workflow runs and logs, identifies root causes, implements minimal fixes, and pushes to a fix branch.
- **[create-pull-request](.agents/skills/create-pull-request)** — Create a GitHub pull request following project conventions. Handles commit analysis, branch management, and PR creation using the gh CLI tool.
- **[docs-update](.agents/skills/docs-update)** — Update user-facing documentation when code changes. Analyzes recent commits for documentation needs and keeps docs in sync with the codebase.
- **[github-bug-report-triage](.agents/skills/github-bug-report-triage)** — Triage GitHub bug reports for actionability. Evaluates whether a bug issue has sufficient detail and identifies missing information from the reporter.
- **[github-issue-dedupe](.agents/skills/github-issue-dedupe)** — Detect duplicate GitHub issues using semantic search and keyword matching.
- **[mcp-builder](.agents/skills/mcp-builder)** — Build high-quality MCP (Model Context Protocol) servers that let LLMs interact with external services through well-designed tools.
- **[scheduler](.agents/skills/scheduler)** — Schedule on-device reminders and local actions. Set personal reminders or run lightweight local tasks at a specific time or interval.
- **[seo-aeo-audit](.agents/skills/seo-aeo-audit)** — Optimize for search engine visibility, ranking, and AI citations (SEO + AEO).
- **[slack-qa-investigate](.agents/skills/slack-qa-investigate)** — Investigate and answer repository questions in read-only mode. Provides research-backed answers that require codebase and documentation investigation.
- **[terraform-style-check](.agents/skills/terraform-style-check)** — Generate Terraform HCL code following HashiCorp's official style conventions and best practices.
- **[web-accessibility-audit](.agents/skills/web-accessibility-audit)** — Audit web applications for WCAG accessibility compliance. Identifies common violations and provides remediation guidance.
- **[web-performance-audit](.agents/skills/web-performance-audit)** — Audit web performance using Chrome DevTools MCP. Profile, debug, or optimize page load performance and Lighthouse scores.
- **[webapp-testing](.agents/skills/webapp-testing)** — Test local web applications with Playwright. Verify frontend functionality, debug UI behavior, and capture browser screenshots.

## Contributing

Contributions are welcome! See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on adding skills.

## Learn More

- [Agent Skills Specification](https://agentskills.io)
- [Oz Skills Documentation](https://docs.warp.dev/agent-platform/cloud-agents/skills-as-agents)
