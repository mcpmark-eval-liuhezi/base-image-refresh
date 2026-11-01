# Training Stack Refresh — Debian Base-Image Cadence & Upstream PR Load

Annual base-image refresh review notes for the lab training stack (huggingface/transformers).

## Debian release cadence

- Debian 13 "Trixie" — version 13.0 initially released: **2025-08-09** (Debian 13.7 follow-up release 2026-09-12).
- Debian 12 "Bookworm" — version 12.0 initially released: **2023-06-10** (Debian 12.15 follow-up release 2026-07-11).
- Source pages: https://www.debian.org/releases/trixie/ and https://www.debian.org/releases/bookworm/ (release index: https://www.debian.org/releases/).
- Day gap between the two initial releases (2023-06-10 → 2025-08-09): **791 days** (exact arithmetic: 366 + 365 + 20 + 31 + 9).

## Upstream pull-request load

- Open pull requests in huggingface/transformers: **657**.
- Open PRs mentioning "llama": **87**.
- "llama" share of the open backlog: 87 / 657 × 100 = 13.24200913242009% → **13.2%** (one decimal place).
- Weeks to clear the entire open backlog at 5 PRs/day: 657 / 5 = **131.4 weeks** (one decimal place).

## Links

- Upstream repository: https://github.com/huggingface/transformers
- Debian releases index: https://www.debian.org/releases/
- Debian Bookworm (12) release page: https://www.debian.org/releases/bookworm/
- Debian Trixie (13) release page: https://www.debian.org/releases/trixie/
