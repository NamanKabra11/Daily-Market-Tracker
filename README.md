# Daily Market Ledger

A news-driven equity research and paper-trading method, packaged as a Claude skill.

Share a business news (PDF, photos, links or text) and Claude turns it into a
market brief and rule-based stock calls, each tracked against the Nifty 50.

## How it works
- **Reads the news for second-order effects**: who is hit one step away from the headline,
  what is new versus already priced in, and how big it is for the company.
- **Rule-based calls**: written thesis, own target and stop-loss (minimum 1.5:1
  reward-to-risk), fixed holding period, LONG or AVOID.
- **Honest tracking**: entry after 9:30 IST, hourly price checks, exits at the
  stop/target level (gap-aware), held through results, post-mortem on every close.
- **Benchmarked** against the Nifty 50 over the same period.

## What's inside
- `SKILL.md`: the method (story selection, call rules, entry/stop/gap rules, scoring)
- `assets/dashboard.html`: the ledger dashboard (Today, Call ledger, Review)
- `assets/pdf-lib.min.js`: splits newspaper PDFs over 20 MB
- `references/`: templates for the hourly price tracker and the morning paper reader

## Install
1. Download `daily-market-ledger-skill.zip` from **Releases** (right side of this page).
2. In Claude: Settings → Capabilities → Skills → Upload skill → choose the zip.
3. Share a business paper, photo, link or article text in a chat. Claude asks before creating your ledger.

*Paper trading for learning. Not investment advice.*
