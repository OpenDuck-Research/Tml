# Contributing to Tml

Thanks for being interested in Tml.

This project is small, explicit, and security-focused. If you want to contribute, keep the scope tight and keep the project’s goals in mind: install browser software safely, verify it properly, and avoid adding hidden behavior or convenience features that undermine trust.

## Before you open a PR

Please read:
- `README.md`
- `DEVELOPMENT.md`
- `SECURITY.md`

If your idea changes the project’s security model, the browser source policy, installation flow, or verification rules, it should be discussed first.

## Good contributions

These are the kinds of changes that fit well here:
- bug fixes with a clear cause
- better validation or safety checks
- documentation that makes behavior clearer
- small improvements to reliability or maintainability

This project does not need broad refactors or “cleanup” changes unless they directly support the fix or feature.

## Things to avoid

Please do not:
- add telemetry or tracking
- silently relax security checks
- guess browser state in ways that may be wrong
- introduce mirror or fallback behavior without a good reason
- add dependencies just because they are convenient
- make big scope changes unrelated to the issue

If a change touches downloads, verification, extraction, AppArmor, or browser source handling, it needs extra care.

## Reporting bugs

Open an issue with:
- what happened
- what you expected to happen
- the browser involved
- your OS and environment
- steps to reproduce
- any logs or screenshots if relevant

If it is a security issue, do not post it publicly. Use the process in `SECURITY.md`.

## Pull requests

Keep pull requests focused.

A good PR:
- solves one problem
- is easy to review
- explains why the change matters
- includes testing or validation notes
- does not mix unrelated cleanup into the same patch

If a change affects security-sensitive behavior, explain the risk and what was checked.

## Review standards

Changes will be judged by:
- correctness
- security impact
- fit with the project’s goals
- clarity
- maintainability

The project is intentionally conservative. A change that sounds clever but weakens the trust model is not an improvement.

## Code of conduct

Be respectful, constructive, and technical. We care more about the actual code and the risk model than about style debates or ego.

## License

By contributing, you agree that your contributions will be licensed under the MIT License.