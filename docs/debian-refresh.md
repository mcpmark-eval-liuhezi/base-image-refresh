# Training stack refresh — Debian cadence and upstream PR load

Notes for the annual base-image refresh review.

## Debian release cadence

The two most recent stable releases listed on the Debian releases index:

| Release | Initial (x.0) release date |
| --- | --- |
| Debian 13 "trixie" | August 9th, 2025 |
| Debian 12 "bookworm" | June 10th, 2023 |

Day gap between the two initial release dates: **791 days** (roughly 2 years, 2 months).

Arithmetic, for the record: 2023-06-10 -> 2025-08-09
= 204 days remaining in 2023 + 366 days (2024, a leap year) + 221 days elapsed in 2025
= 791 days.

Dates are the initial x.0 releases as stated on each release's own page, not point releases.

## Upstream pull-request load

Pinned upstream stack: `huggingface/transformers`

- Open pull requests (total): **612**
- Open pull requests mentioning "llama": **81**
- "llama" share of open PRs: 81 / 612 = 13.23529411764706% ≈ **13.2%**
- Triage capacity: 5 PRs/day, 7 days a week -> 612 / 5 = 122.4 days = 122.4 / 7 = 17.485714285714288 weeks ≈ **17.5 weeks** to clear the entire open backlog.

Takeaway: the open backlog is large and llama-related work accounts for a meaningful slice of it, so the refresh window should plan for dependency churn.

## Links

- Upstream repository: https://github.com/huggingface/transformers
- Debian releases index: https://www.debian.org/releases/
- Debian 13 (trixie) release page: https://www.debian.org/releases/trixie/
- Debian 12 (bookworm) release page: https://www.debian.org/releases/bookworm/