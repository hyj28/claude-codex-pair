# Security policy

This project coordinates two coding agents, invokes headless commands, and installs skills
into a user-selected Claude Code directory. A quiet change to those boundaries can be more
dangerous than an obvious failure.

## Reporting a vulnerability

Use [GitHub's private vulnerability reporting](https://github.com/hyj28/claude-codex-pair/security/advisories/new)
for sandbox widening, command injection, unintended auto-activation, destructive installer
behavior, credential exposure, or a workflow that pushes, merges, or changes sensitive data
without the documented human gate.

Include the affected version, platform, relevant CLI versions, the smallest safe reproduction,
and the boundary you expected. Remove tokens, credentials, private prompts, and repository
content before sending a report.

You should receive an acknowledgement within seven days. Please allow time for a fix and a
coordinated release before publishing details.

## Supported versions

Security fixes target the latest tagged release and `main`. Older pre-1.0 releases are not
guaranteed to receive backports.
