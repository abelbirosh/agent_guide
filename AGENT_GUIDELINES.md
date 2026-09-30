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
