# Agent Guidelines

## Architecture

- Before writing any code, split the software into modular components, each in its own directory or subdirectory.

## Testing

- Unit tests, if written, must be written exclusively before development begins, not after.
- After development, all testing must be functional tests. Unit tests are allowed at this stage only for edge cases and malformed-input handling.

## CI/CD

- Every repo must have CI/CD running on pull requests, including linting.
- PRs that fail any mandatory test suite must be blocked from merging.
- Branch protection must be active on `main`.

## Commits and PRs

- Every commit message must start with one of `feat:`, `fix:`, `docs:`, `style:`, `test:`, `chore:`, or `revert:`, chosen according to the [Conventional Commits](https://www.conventionalcommits.org/) standard.
- Every PR must include a change log with three parts: **System before**, **Task**, and **System after**.
- PR descriptions must be concise and bulleted.
