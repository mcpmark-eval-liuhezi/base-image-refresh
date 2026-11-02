# Base Image Refresh — Research Notes

Annual base-image refresh review for the training stack (Debian base OS cadence and upstream PR load).

## Debian release cadence

- Debian 13 'Trixie' initial release (13.0): 2025-08-09 (August 9th, 2025)
- Debian 12 'Bookworm' initial release (12.0): 2023-06-10 (June 10th, 2023)
- Days between 2023-06-10 and 2025-08-09: 791 days

Source pages:
- https://www.debian.org/releases/trixie/ (Debian 13.0 initially released on August 9th, 2025)
- https://www.debian.org/releases/bookworm/ (Debian 12.0 initially released on June 10th, 2023)
- https://www.debian.org/releases/ (releases index listing 13 Trixie 2025-08-09 and 12 Bookworm 2023-06-10)

## Upstream pull-request load

- Open pull requests in huggingface/transformers: 655
- Open pull requests mentioning 'llama': 87
- 'llama' share of open PRs: 13.3% (87 / 655 * 100 = 13.282442748091603%)
- Weeks to clear entire open backlog at 5 PR/day: 18.7 weeks (655 / 5 = 131 days; 131 / 7 = 18.714285714285715 weeks)

## Links

- Upstream repository: https://github.com/huggingface/transformers
- Debian releases index: https://www.debian.org/releases/
- Debian Trixie release page: https://www.debian.org/releases/trixie/
- Debian Bookworm release page: https://www.debian.org/releases/bookworm/
