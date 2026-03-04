# Contribution Guidelines (Internal)

## 1. Purpose

These guidelines standardize how changes are proposed, reviewed, and merged to ensure maintainability, reliability, and security.

## 2. Scope

Applies to all changes to this repository, including:

- code, tests, documentation
- CI/CD workflows
- configuration and infrastructure-as-code

## 3. Access and Branching Model

- Default branch: `main`
- Branch naming:
  - `feature/<ticket>-<short-description>`
  - `fix/<ticket>-<short-description>`
  - `chore/<ticket>-<short-description>`
- Direct pushes to protected branches are not permitted unless explicitly authorized.

## 4. Commit Message Standard

Use clear, auditable commit messages. Recommended format:

- `type(scope): summary (TICKET-123)`

Where `type` ∈ `feat|fix|docs|refactor|test|chore`.

## 5. Pull Request Requirements

All changes must be delivered via Pull Request.

A Pull Request must include:

- Purpose and context (what/why)
- Testing evidence (what was executed and results)
- Risk assessment (areas affected, backward compatibility)
- Operational notes (migration steps, flags, rollout/rollback), where applicable

### 5.1 Quality gates (expected)

A PR is eligible for merge only if:

- Required CI checks are successful
- Required reviews are approved (incl. CODEOWNERS where configured)
- Review conversations are resolved
- No secrets or sensitive data are introduced

## 6. Testing and Local Validation

Run the applicable local checks before requesting review. Document the standard commands for this repository below (adjust):

- Setup: `make setup`
- Lint: `make lint`
- Tests: `make test`
- Build: `make build`

## 7. Security and Data Handling

- Do not commit credentials, tokens, private keys, certificates, or proprietary customer data.
- Use sanitized/anonymous test data only.
- If you suspect a security issue, follow [SECURITY.md](./SECURITY.md).

## 8. Ownership and Support

- Owner team: **@TU-ORG/TEAM**
- Support channel: **#team-canal**
