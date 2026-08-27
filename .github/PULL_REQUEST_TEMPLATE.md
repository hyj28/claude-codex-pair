## What changed

<!-- Describe the workflow problem and the user-visible behavior after this change. -->

## Boundaries

- [ ] The skills still activate only when explicitly invoked
- [ ] Implementation and review sandboxes remain explicitly pinned
- [ ] Review remains fresh-context and read-only
- [ ] Gate outcomes are based on command evidence, not agent claims
- [ ] Fix and review loops remain bounded
- [ ] Merging, pushing, and sensitive operations remain human decisions

## Verification

- [ ] `shellcheck install.sh`
- [ ] `bash -n install.sh`
- [ ] Temporary-directory installer regression check
- [ ] Skill frontmatter and relative links checked

## Evidence

<!-- Add the exact invocation and concise, redacted transcript or gate output. -->
