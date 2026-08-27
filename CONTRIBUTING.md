# Contributing

Thanks for helping make the pair workflow more predictable and easier to trust.

Before changing behavior, read [WORKFLOW.md](WORKFLOW.md). The following guarantees are
load-bearing and should not be weakened quietly:

- both skills activate only when explicitly invoked;
- implementation runs with an explicitly pinned workspace sandbox and no approvals;
- review runs in fresh, read-only context;
- gate results come from commands and observable evidence, not agent claims;
- loops are bounded, and merging or pushing remains a human decision.

Keep pull requests focused and explain the workflow failure or user friction they address.
For a behavior change, include the exact invocation and the expected transcript or gate
outcome. Before opening a pull request, run:

```bash
shellcheck install.sh
bash -n install.sh
```

Also install into a temporary `CLAUDE_SKILLS_DIR` and confirm that `pair/SKILL.md`,
`pair/WORKFLOW.md`, and `pair-review/SKILL.md` are present. CI repeats this regression
check, validates skill frontmatter, and verifies every relative Markdown link.

Security-sensitive findings about sandbox widening, unintended activation, or destructive
installation behavior should follow [SECURITY.md](SECURITY.md), not a public issue.
