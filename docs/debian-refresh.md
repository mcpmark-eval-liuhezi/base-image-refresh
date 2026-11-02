# Training Stack Refresh — Debian Cadence and Upstream PR Load

Annual base-image refresh review for the lab training stack (huggingface/transformers).

## Debian release cadence

- Debian 13 'Trixie' — initial release (Debian 13.0): **2025-08-09**
- Debian 12 'Bookworm' — initial release (Debian 12.0): **2023-06-10**
- Day gap between the two initial releases: **791 days**

Sources:
- https://www.debian.org/releases/trixie/ (Debian 13.0 initially released on August 9th, 2025)
- https://www.debian.org/releases/bookworm/ (Debian 12.0 initially released on June 10th, 2023)
- https://www.debian.org/releases/ (index of releases: 13 Trixie 2025-08-09; 12 Bookworm 2023-06-10)

## Upstream pull-request load

- Open pull requests in huggingface/transformers: **655**
- Open pull requests mentioning 'llama': **87**
- 'llama' share of open PRs: 87 / 655 * 100 = 13.282442748091603% ≈ **13.3%**
- Weeks to clear the entire open backlog at 5 PR/day: 655 / 5 = **131.0 weeks**

Sources:
- https://github.com/huggingface/transformers (PR search: is:open -> 655; is:open llama -> 87)

## Links

- Upstream repository: https://github.com/huggingface/transformers
- Debian releases index: https://www.debian.org/releases/
- Debian 13 'Trixie' release page: https://www.debian.org/releases/trixie/
- Debian 12 'Bookworm' release page: https://www.debian.org/releases/bookworm/
