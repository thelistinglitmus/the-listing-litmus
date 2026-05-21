# The Listing Litmus

A community-maintained block list of staffing firms, recruiter shops, and "Easy Apply" listings on LinkedIn that show patterns inconsistent with legitimate recruitment: bulk job posting, AI-data-harvesting interview pipelines, India-fronted US-LLC structures, resume harvesting with no real placement, atypical compensation framing, and similar.

The name is the project's job: a litmus test you can run on a listing before you spend half an hour tailoring a resume for it.

**This is not legal advice and not a takedown list.** Every entry is based on observable facts (active listing counts, employee counts, posting cadence, pay format) and third-party reports (Glassdoor patterns, BBB complaints, Scam Detector / Scamdoc scores, Reddit threads, blog writeups). Read the sources and decide for yourself.

## What this is

A regularly-updated CSV and human-readable markdown list of companies that consistently fail a vetting checklist (see [VETTING.md](VETTING.md)). Entries are added only when at least three independent third-party signals corroborate the pattern.

Companion to the [weekly digest on Substack](https://thelistinglitmus.substack.com/). The digest narrates the patterns; this repo holds the raw data.

## How the data is organized

- **[`SkippedCompanies.md`](SkippedCompanies.md)** — human-readable list. Each entry has: company name, date flagged, reason, observable facts, third-party sources, links.
- **[`SkippedCompanies.csv`](SkippedCompanies.csv)** — machine-readable database with the same data, structured for sorting / filtering / programmatic use.
- **[`watchlist.md`](watchlist.md)** — companies under investigation but lacking the threshold for the main list.
- **[`VETTING.md`](VETTING.md)** — the checklist used to evaluate each new candidate before adding to the list.

## How to use the block list

- **Job seekers**: search this repo before applying to a company you don't recognize. If they're on the list, the sources will tell you why.
- **Programmatic filtering**: import `SkippedCompanies.csv` into your own job search tooling to filter listings before they reach your queue.
- **Researchers and journalists**: the structured data is intended to be citable. Please reference the linked third-party sources rather than this repo as the original claim.

## How to contribute

Pull requests welcome with the following format:

1. Add a row to `SkippedCompanies.csv` with all required fields.
2. Add a corresponding entry to `SkippedCompanies.md` with the full writeup.
3. Include at least two third-party sources (Glassdoor, BBB, Scam Detector, Reddit thread, blog writeup, news article). Single-source submissions go to `watchlist.md` until corroborated.
4. Stick to pattern-based language. "Company X shows pattern Y, see sources" — not "Company X is a scam."

For sensitive submissions where you don't want to PR publicly, email gideontrace@proton.me with the same source documentation.

## Cadence

The Substack digest goes out roughly weekly when there are 3+ new entries. If no new entries accumulate over six weeks, a quiet-period reflection digest covers what the absence tells us about the landscape.

## Author

Maintained by **Gideon Trace**.

## License

Block list data is licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](LICENSE). Attribution requested.
