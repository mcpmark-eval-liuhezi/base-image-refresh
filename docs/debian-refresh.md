# Training Stack Refresh — Debian Cadence and Upstream PR Load

Annual base-image refresh review for the lab training stack (huggingface/transformers pinned).

## Debian release cadence

- Debian 13 'Trixie' (13.0) initial release: **2025-08-09** (August 9, 2025)
- Debian 12 'Bookworm' (12.0) initial release: **2023-06-10** (June 10, 2023)
- Day gap (Trixie 13.0 minus Bookworm 12.0): **791 days**

Computed exactly: 2023-06-10 → 2024-06-10 = 366 days (2024 is a leap year, Feb 29 included);
2024-06-10 → 2025-06-10 = 365 days; 2025-06-10 → 2025-08-09 = 20 (rest of June) + 31 (July) + 9 (Aug) = 60 days.
Total = 366 + 365 + 60 = 791 days.

Sources:
- https://www.debian.org/releases/trixie/ (states: "Debian 13.0 was initially released on August 9th, 2025.")
- https://www.debian.org/releases/bookworm/ (states: "Debian 12.0 was initially released on June 10th, 2023.")
- https://www.debian.org/releases/ (releases index: 13 Trixie 2025-08-09; 12 Bookworm 2023-06-10)

## Upstream pull-request load

- Open pull requests in huggingface/transformers: **655**
- Open PRs mentioning 'llama': **87**
- 'llama' share of open PRs: 87 / 655 * 100 = 13.282442748091603% ≈ **13.3%**
- Weeks to clear entire open backlog at 5 PRs/day: 655 / 5 = 131 days; 131 / 7 = 18.714285714285715 ≈ **18.7 weeks**

Sources:
- https://github.com/huggingface/transformers (PR search: is:open repo:huggingface/transformers → 655 total)
- https://github.com/huggingface/transformers (PR search: is:open llama repo:huggingface/transformers → 87 total)

## Links

- Upstream repository: https://github.com/huggingface/transformers
- Debian releases index: https://www.debian.org/releases/
- Debian 13 'Trixie' release page: https://www.debian.org/releases/trixie/
- Debian 12 'Bookworm' release page: https://www.debian.org/releases/bookworm/
