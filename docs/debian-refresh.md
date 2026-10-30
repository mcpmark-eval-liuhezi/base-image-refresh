# Training stack refresh — Debian cadence and upstream PR load

Notes for the annual base-image refresh review.

## Debian release cadence

The two most recent stable releases listed on the Debian releases index:

| Release | Initial (x.0) release date |
| --- | --- |
| Debian 13 "trixie" | August 9th, 2025 |
| Debian 12 "bookworm" | June 10th, 2023 |

Both dates are the initial x.0 releases as stated on each release's own page (not point releases):

- Debian 13.0 "trixie": initially released on August 9th, 2025 — see https://www.debian.org/releases/trixie/
- Debian 12.0 "bookworm": initially released on June 10th, 2023 — see https://www.debian.org/releases/bookworm/

Day gap between the two initial release dates: **791 days** (2023-06-10 -> 2025-08-09).

Exact arithmetic for the record:

- 204 days remaining in 2023 (2023-06-10 through 2023-12-31)
- + 366 days for 2024 (2024 is a leap year, so the interval includes 2024-02-29)
- + 221 days elapsed in 2025 (2025-01-01 through 2025-08-09: 31+28+31+30+31+30+31+9)

204 + 366 + 221 = 791 days. (Equivalently: two full years of 366 + 365 = 731 days, plus 60 days from 2025-06-10 to 2025-08-09, = 791 days.)

Roughly 2 years and 2 months between the two initial x.0 releases.

## Upstream pull-request load

Pinned upstream stack: `huggingface/transformers`

- Open pull requests (total): **649**
- Open pull requests mentioning "llama": **84**
- "llama" share of open PRs: 84 / 649 × 100 = 12.942989214175654% ≈ **12.9%**
- Triage capacity assumed at 5 PRs/day, 7 days a week: 649 / 5 = 129.8 days = 129.8 / 7 = **18.542857142857144** weeks ≈ **18.5 weeks** to work through the entire open backlog.

Takeaway: the open backlog is large and llama-related work accounts for roughly oneventh of it, so the refresh window should plan for dependency churn.

## Links

- Upstream repository: https://github.com/huggingface/transformers
- Debian releases index: https://www.debian.org/releases/
- Debian 13 (trixie) release page: https://www.debian.org/releases/trixie/
- Debian 12 (bookworm) release page: https://www.debian.org/releases/bookworm/
