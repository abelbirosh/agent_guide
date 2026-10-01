# Agent Guidelines

## Architecture

- Before writing any code, split the software into modular components, each in its own directory or subdirectory.

## Fixes

- Resolve bugs with the smallest change that fixes the issue.

## Testing

- Unit tests, if written, must be written exclusively before development begins, not after.
- After development, all testing must be functional tests. Unit tests are allowed at this stage only for edge cases and malformed-input handling.

## CI/CD

- Every repo must have CI/CD running on pull requests, including linting.
- PRs that fail any mandatory test suite must be blocked from merging.
- Branch protection must be active on `main`.
- If the repo has separate prod and dev branches, push only to the dev branch.

## Commits and PRs

- Every commit message must start with one of `feat:`, `fix:`, `docs:`, `style:`, `test:`, `chore:`, or `revert:`, chosen according to the [Conventional Commits](https://www.conventionalcommits.org/) standard.
- Each commit must contain exactly one functional change. Stack PRs when needed to keep changes separate.
- Every PR must include a change log with three parts: **System before**, **Task**, and **System after**.
- PR descriptions must be concise and bulleted.

## Documentation

- When a structural change warrants it, update the README and the download/install instructions to match.
- Maintain a change log in the project's README with one row per PR:

  | Date | PR ID | System Before | Task | System After | Status |
  |---|---|---|---|---|---|

## Token Budget

- Track token usage whenever it is available.
- Once the user's requirements are met, stop iterating. Don't keep spending a large share of the token budget on further improvements.
