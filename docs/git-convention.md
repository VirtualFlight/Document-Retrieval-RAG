# Repository Conventions

This document defines the coding, branching, commit, and pull request conventions for this repository.

## Branching Strategy

This repository uses a **`main` + feature branches** workflow.

### Protected Branch

- **`main`**
  - Always stable and deployable.
  - Only merged features that are complete and tested.
  - Should be protected (require pull request reviews).

### Branch Naming Convention

All branches must follow this naming pattern:

```text
<type>/<short-description>
```

Where `<type>` is one of:

| Type | Description |
|------|-------------|
| `feat` | New feature or functionality |
| `fix` | Bug fix |
| `docs` | Documentation-only changes |
| `chore` | Tooling, config, repo maintenance |
| `refactor` | Code refactor without behavior change |
| `test` | Adding or updating tests |
| `ci` | CI/CD configuration changes |

### Examples

```bash
feat/document-ingestion
feat/rag-qna
feat/react-chat-ui
feat/deals-endpoint
fix/search-encoding
fix/sql-connection
docs/readme-setup
docs/architecture-diagram
chore/add-gitignore
chore/azure-env-example
refactor/ingest-module
test/rag-unit-tests
ci/github-actions-deploy
```

### Workflow

1. Create a feature branch from `main`:
   ```bash
   git checkout main
   git pull
   git checkout -b feat/<description>
   ```
2. Develop and commit on the feature branch.
3. Open a pull request to merge into `main`.
4. After review and approval, squash-merge the branch into `main`.
5. Delete the feature branch after merging.

---

## Commit Message Convention

This repository follows the **Conventional Commits** specification.

### Format

```text
<type>(<scope>): <short description>
```

### Types

| Type | Description |
|------|-------------|
| `feat` | New feature |
| `fix` | Bug fix |
| `docs` | Documentation only |
| `chore` | Maintenance, config, tooling |
| `refactor` | Code refactor (no behavior change) |
| `test` | Adding or updating tests |
| `ci` | CI/CD changes |


## Pull Request Convention

All changes to `main` must be made via pull requests.

### PR Title

Use the same format as commit messages:

```text
<type>(<scope>): <short description>
```

Examples:

- `feat(backend): document ingestion pipeline`
- `feat(frontend): chat UI for RAG Q&A`
- `docs(readme): add architecture and setup docs`

### PR Description Template

```markdown
## Summary
Briefly describe what this PR does.

## Changes
- Bullet list of key changes
- Mention new files or major refactors

## How to Test
1. Steps to run locally
2. What endpoints/pages to hit
3. Expected behavior

## Screenshots / Demo (if applicable)
- Add screenshots of UI or terminal output

## Checklist
- [ ] Code runs locally
- [ ] No sensitive data (keys, secrets) committed
- [ ] README updated if needed
- [ ] Related docs updated (architecture, user requirements)
```

---