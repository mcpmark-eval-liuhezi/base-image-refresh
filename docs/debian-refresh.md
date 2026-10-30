# Training stack refresh — Debian cadence and upstream PR load

Notes for the annual base-image refresh review.

## Debian release cadence

The two most recent stable releases listed on the Debian releases index:

| Release | Initial (x.0) release date | Source |
| --- | --- | --- |
| Debian 13 "trixie" | August 9th, 2025 | Debian 13.0 initially released on August 9th, 2025 (per the trixie release page; the latest point release, 13.7, is later and is not counted) |
| Debian 12 "bookworm" | June 10th, 2023 | Debian 12.0 initially released on June 10th, 2023 (per the bookworm release page; the latest point release, 12.15, is later and is not counted) |

Both dates come from the release's own page on the Debian Releases Archive, not from a point release.

Day gap between the two initial (x.0) release dates: **791 days** (2023-06-10 -> 2025-08-09).

Arithmetic, for the record:
- 2023-06-10 to end of 2023: 204 days remaining in 2023
- 2024 (leap year): 366 days
- 2025-01-01 to 2025-08-09: 221 days elapsed in 2025
- 204 + 366 + 221 = 791 days

That is roughly 2 years and 2 months — useful for planning when the next base-image refresh will be due.

## Upstream pull-request load

Pinned upstream stack: `huggingface/transformers`.

- Open pull requests (total, live lookup): **649**
- Open pull requests mentioning "llama": **84**
- "llama" share of open PRs: 84 / 649 = 12.942989...% ≈ **12.9%**
- Triage capacity assumed at 5 PRs/day, 7 days a week -> 649 / 5 = 129.8 days = 129.8 / 7 = **18.5 weeks** to work through the entire open backlog.

Takeaway: the open backlog is large and llama-related work accounts for a meaningful slice of it, so the refresh window should plan for dependency churn.

## Links

- Upstream repository: https://github.com/huggingface/transformers
- Debian releases index: https://www.debian.org/releases/
- Debian 13 (trixie) release page: https://www.debian.org/releases/trixie/
- Debian 12 (bookworm) release page: https://www.debian.org/releases/bookworm/
