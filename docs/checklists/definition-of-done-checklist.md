# Definition of Done Checklist

An item is considered **Done** only when all applicable boxes below are checked.

---

## Functional & Acceptance
- [ ] Acceptance criteria are met and verified
- [ ] Product Manager / PdM has signed off on the feature behaviour
- [ ] Edge cases and error states are handled

## Testing
- [ ] Unit tests written and passing
- [ ] Integration tests written and passing (where applicable)
- [ ] End-to-end / smoke tests pass for critical flows
- [ ] No regressions introduced in existing test suite

## Security & Compliance
- [ ] Security scan (SAST/dependency scan) passing in CI
- [ ] No new high or critical vulnerabilities introduced
- [ ] Sensitive data handling reviewed (no secrets in code/logs)

## Code Quality & Review
- [ ] Code reviewed and approved by at least one peer
- [ ] CI checks (lint + tests) passing
- [ ] PR linked to the relevant issue with acceptance criteria referenced

## Documentation
- [ ] Inline code comments added for complex logic
- [ ] Relevant process docs or README updated if behaviour changes
- [ ] API / interface changes reflected in documentation

## Release Readiness
- [ ] Feature flag / rollout plan considered if applicable
- [ ] Deployment steps documented or automated
- [ ] Rollback plan identified

---

> Refer to [octoacme-release-and-deployment.md](../octoacme-release-and-deployment.md) for full release gate requirements.
