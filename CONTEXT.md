# sharkdp/fd context
> refreshed 2026-10-11 | upstream default: master @ 14dcd92fb76ca0ebc2e82671a275f67c790d25fc

## Identity & policies
- upstream: sharkdp/fd, default branch master, primary language Rust, English-first (yes — README/docs in English)
- CLA/DCO: none (no CLA bot, no DCO in CONTRIBUTING)
- AI-assisted PR policy: CONTRIBUTING point 4 requires indicating if an AI tool was used; passport flags ai_disclosure_required=false (fork PRs carry no AI mention; disclosure at Oli's manual promotion)
- signed commits required: no
- PR template: none (no .github/PULL_REQUEST_TEMPLATE.md) — use pipeline 3-section fallback body
- external tracker: github

## Conventions (verified from merged PRs)
- branch naming: `fix-<kebab>`, `docs-<kebab>`, `chore-<kebab>`, `tests/<kebab>`, `fix/<kebab>`, `docs/<kebab>` (e.g. fix-readme-example, docs-msrv, fix-readme-bash-fence, fix-readme-number-format)
- commit style: conventional-ish (`fix:`, `docs:`, `chore:`, `refactor:`)
- test command: `cargo test`; lint: `cargo clippy`; CI: build+test matrix across platforms
- CONTRIBUTING: open an issue first for anything beyond a small fix; typo/doc fixes don't need CHANGELOG entry
- outside PRs get merged: yes — recent external merges (nikolauspschuetz, cmelaro, parneetsingh022, mahirhir, bonanza127, WilliamLeony, kobihikri, stevenwalton, wyf027)

## Maintainer picture
- active maintainer: Thayne McCombs (tmccombs) — merges regularly, fast turnaround
- areas actively worked: jemalloc, error handling, changelog/release chores

## Issue-area health
- 40+ open issues, 20+ open PRs (mostly dependabot + a few feature PRs); refreshed 2026-09-30
- healthy, responsive; small doc/typo PRs from outsiders have merged recently

## Gap ledger (dedupe — READ FIRST, never re-pick)
- 2026-09-03: trivial-fix pass — 5 fixes (CHANGELOG typos calander/ouput, README "options … option" x2, fd.1 regex link 1.0.0→latest). PR #1 opened in fork (docs/trivial-fixes). DONE.
- 2026-09-30: self-found gap (repo-audit) — zsh completion `contrib/completion/_fd` omits `--format`, `--ignore-contain`, `--quiet`/`--has-results`. PR opened in fork (docs/zsh-completion-options). DONE.
- 2026-10-11: trivial-fix pass — 4 fixes in 4 files (README "inplace"->"in place", CHANGELOG "officla"->"official", scripts/create-deb.sh "all of finds powerful"->"find's", tests/tests.rs "failde"->"failed"). Exhaustive sweep (codespell, typos-cli, doubled-word/possessive grep, link liveness) found nothing else genuine; AU/UK spellings left as-is; `gawk -i inplace` is a real flag. PR #9 opened in fork (docs/minor-typo-fixes). DONE.

## Mined gaps (discovered, not yet attempted)
- 2026-09-30 zsh completion omits three CLI options present in `fd --help` (`--format <fmt>`, `--ignore-contain <name>`, `--quiet`/`-q` alias `--has-results`) — status: attempted (PR opened 2026-09-30, docs/zsh-completion-options).
