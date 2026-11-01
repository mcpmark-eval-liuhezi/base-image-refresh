# Training Stack Refresh — Debian Cadence and Upstream PR Load

Annual base-image refresh review notes for the lab training stack.

## Debian release cadence

Base OS cadence for our images: Debian. The two most recent stable releases listed
on the official Debian releases index are Debian 13 'Trixie' and Debian 12 'Bookworm'.

- Debian 13 'Trixie' — initial release (version 13.0): **2025-08-09** (August 9th, 2025)
- Debian 12 'Bookworm' — initial release (version 12.0): **2023-06-10** (June 10th, 2023)

Day gap between the two initial release dates (2023-06-10 to 2025-08-09):
**791 days** (366 + 365 + 20 + 31 + 9).

## Upstream pull-request load

Our stack is pinned to huggingface/transformers.

- Open pull requests in huggingface/transformers: **657**
- Open pull requests mentioning 'llama': **87**
- Share of open PRs mentioning 'llama': **13.2%** (87 / 657 * 100 = 13.24200913242009)
- Weeks to clear the entire open backlog at 5 PR/day: **18.8 weeks**
  (657 / 5 = 131.4 days; 131.4 / 7 = 18.771428571428572 weeks)

## Links

- Upstream repository: https://github.com/huggingface/transformers
- Debian releases index: https://www.debian.org/releases/
- Debian 'trixie' (Debian 13) release page: https://www.debian.org/releases/trixie/
- Debian 'bookworm' (Debian 12) release page: https://www.debian.org/releases/bookworm/
