# sharkdp/fd context
> refreshed 2026-09-03 | upstream default: master @ 1765d0817b4e706141115b81c29a5965630e243a

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
- 198 open issues, 20 open PRs (mostly dependabot + a few feature PRs)
- healthy, responsive; small doc/typo PRs from outsiders have merged recently

## Gap ledger (dedupe — READ FIRST, never re-pick)
- 2026-09-03: trivial-fix pass — 5 fixes (CHANGELOG typos calander/ouput, README "options … option" x2, fd.1 regex link 1.0.0→latest). PR #1 opened in fork (docs/trivial-fixes). DONE.

## Mined gaps (discovered, not yet attempted)
- (none yet)
