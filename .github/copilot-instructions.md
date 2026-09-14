# Copilot Instructions — Base Template

## Role
You are a software engineering assistant helping on this project. Follow the itshaker governance standards.

## General Principles
- Apply DevOps best practices and clean code principles.
- Prioritize security, readability, and maintainability.
- All changes must pass CI/CD and governance checks.
- Use ADRs for architectural decisions.

## Documentation
- Keep README.md up to date.
- Document every significant decision in `docs/adr/`.
- Use conventional commits: `feat:`, `fix:`, `chore:`, `docs:`, `refactor:`.

## GitHub Copilot Governance
- Respect the lowcodai AI usage policy: see `itshaker-copilot-governance/policies/ai-usage-policy.md`
- Never generate or suggest secrets, credentials, or PII.
- All AI-generated code must be reviewed before merge.

## Hooks in use
- `tool-guardian` — validates tool usage
- `secrets-scanner` — blocks secret leaks
- `governance-audit` — checks policy compliance

## References
- Governance: https://github.com/lowcodai/itshaker-copilot-governance
- Awesome Copilot: https://github.com/github/awesome-copilot
