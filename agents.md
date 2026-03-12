# Tempus Dominus

<!-- BEGIN PAYREADY STANDARDS — managed centrally, do not edit manually -->

## Working Standards

### Approach
- For changes touching more than 3 files, outline your approach before coding.
- When intent is reasonably clear, act. Only ask for clarification when the request is genuinely ambiguous or involves an irreversible action.
- Prefer focused changes. When a change requires touching multiple files, each changed file should be directly related to the task.
- Do not create new abstractions, refactor, or make "while we're here" edits unless the task explicitly requires it.

### Verification
- Run the repo's test suite after making changes (see Commands below for exact commands).
- Run the linter/formatter. Confirm the build passes.
- Review for correctness and verify nothing downstream will be impacted.

### Delivery
- Summarize what was changed and why.
- List every file modified and what was done in each.
- Flag any assumptions or risks for review.

### Git Rules
- Before committing, check for a CI process. If one exists, run preprocessors and tests and confirm they pass.
- Never commit or push until all checks pass.
- Validate changes by running the service locally before committing.

<!-- END PAYREADY STANDARDS -->

## Overview
Tempus Dominus is a powerful Date/time picker widget built with TypeScript.

## Tech Stack
- **Language:** TypeScript
- **Build:** Rollup, Sass
- **Tests:** Vitest
- **Linting:** ESLint, Prettier

## Commands
| Task | Command |
|------|---------|
| Install | `npm install` |
| Build | `npm run build` |
| Test | `npm test` |
| Test (silent) | `npm run test:silent` |
| Test (coverage) | `npm run test:coverage` |
| Lint | `npm run eslint` |
| Dev server | `npm start` |
| Release | `npm run release` |

## Structure
- `src/` — Source TypeScript and SCSS
- `build/` — Build scripts (Rollup config, utilities)
- `test/` — Vitest test files
- `dist/` — Compiled output (generated)
- `types/` — TypeScript declarations (generated)

<!-- Domain Knowledge: Add integration details, usage patterns, and component API notes here -->
