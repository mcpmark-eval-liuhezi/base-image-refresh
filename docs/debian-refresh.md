# Training stack refresh — research notes

Annual base-image refresh review for the lab training stack.

## Debian release cadence

- Debian 13 'Trixie' (stable): initial release Debian 13.0 on **2025-08-09** (August 9, 2025).
- Debian 12 'Bookworm' (oldstable): initial release Debian 12.0 on **2023-06-10** (June 10, 2023).
- Days between 2023-06-10 and 2025-08-09: **791 days** (366 + 365 + 20 + 31 + 9).

Sources:
- Debian releases index: https://www.debian.org/releases/
- Debian 13 'trixie' release page: https://www.debian.org/releases/trixie/
- Debian 12 'bookworm' release page: https://www.debian.org/releases/bookworm/

## Upstream pull-request load

- Open pull requests in huggingface/transformers: **657**
- Open pull requests mentioning 'llama': **87**
- 'llama' share of open PRs: 87 / 657 x 100 = 13.2420...% -> **13.2%**
- Weeks to clear the entire open backlog at 5 PR/day: 657 / 5 / 7 = 18.7714... -> **18.8 weeks**

## Links

- Upstream repository: https://github.com/huggingface/transformers
- Debian releases index: https://www.debian.org/releases/
- Debian 13 'trixie' release page: https://www.debian.org/releases/trixie/
- Debian 12 'bookworm' release page: https://www.debian.org/releases/bookworm/
