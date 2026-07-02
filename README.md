# oss-workflows

Reusable GitHub Actions workflows (CI + release) shared by my public projects.

- `ci.yml` — secrets scan (gitleaks, blocking), pre-commit checks, per-language test/lint jobs. Call with `uses: tobyrosen/oss-workflows/.github/workflows/ci.yml@v1`.
- `release.yml` — release-please (Conventional Commits → Release PR → tagged GitHub Release) plus per-profile release assets. Call with `uses: tobyrosen/oss-workflows/.github/workflows/release.yml@v1`.

`v1` is a rolling tag: callers pin `@v1` and pick up fixes when the tag moves. Breaking changes get a new major tag.

## License

MIT
