# AGENTS.md

@CLAUDE.md

## Codex Notes

- Read `CLAUDE.md` first; read `rust/CLAUDE.md` before touching the Rust workspace.
- Keep changes small and reviewable. Update tests with behavior changes.
- Do not commit machine-local settings, session files, or cache directories.
- Verify Python changes with `python3 -m unittest discover -s tests`.
- Verify Rust changes from `rust/` with the current CI-equivalent checks:
  - `cargo fmt --all --check`
  - `cargo clippy --workspace --all-targets`
  - `cargo test --workspace -- --test-threads=1`
