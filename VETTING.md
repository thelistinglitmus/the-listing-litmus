# Vetting Checklist

Used to evaluate every new company before adding to [`SkippedCompanies.md`](SkippedCompanies.md) or [`watchlist.md`](watchlist.md).

The threshold for the main block list is **at least three independent red-flag signals** from this checklist. Two signals goes to the watch list for re-vetting on next sighting. One or zero signals: not enough evidence — move on or hold for future sighting.

## The checklist

For any company not already in the block list, run all six checks:

### 1. Search the company name
- `"[Company Name]" scam reddit`
- `"[Company Name]" glassdoor`
- `"[Company Name]" recruiter spam`
- `"[Company Name]" BBB complaints`

Look for: documented patterns from job seekers (not just isolated venting), specific behaviors (resume harvesting, bot interviews, no callbacks), consistent themes across multiple sources.

### 2. Domain sanity check
Visit the company's stated website. Look for:
- Does the domain match the company name? Mismatches like `tek-staffing.com` for "TekNavigators Staffing LLC" are a flag.
- Is there real address information? Watch for nonsense like "Chicago 12, Melborne City, USA".
- Does any listed US phone use a NANPA-assigned area code? Some scam shops use unassigned ranges or international numbers dressed as US ones.
- Lorem ipsum or other placeholder text on a live production site?
- Copyright year that contradicts the company's claimed years-in-business?
- Social media icons that link to "#" or other dead anchors?

### 3. Glassdoor signal (pattern, not just score)
Don't look at the average. Look at the distribution:
- **Real company**: typically 3.0-3.8 stars with a wide range of complaints (work-life, management, pay). 50%+ recommendation rate.
- **Inflated / farmed reviews**: 4.5+ stars on a small unknown company with reviews that all sound similar, posted in clusters, with management responses that defend rather than acknowledge.
- **Scam shop**: low star count or polarized reviews; specific complaints like "they only want my resume," "interview was a bot," "never heard back after 50 spam emails."

### 4. Scam Detector / Scamdoc lookup
- Scam Detector trust score below 30/100: strong block signal
- Scam Detector trust score below 50/100: caution, look for corroborating signals
- Scamdoc trust score below 30%: same threshold
- Recently-registered domain (under 6 months) for a company claiming years of experience: flag

### 5. Bulk-posting check
Search LinkedIn for "[Company Name] jobs" or look at their company page. Count:
- Active listings
- Employee count from their LinkedIn profile

Red flag: 1000+ active listings against fewer than 100 employees. Real recruiters can't process that volume of reqs per employee.

Also check for **title variation** — if the same company is posting 5+ wildly different roles (AD Specialist, Game QA Tester, Notion Specialist, SRE all from one firm) in a short window, that's the "throw spaghetti at the wall to harvest resumes" pattern.

### 6. r/recruitinghell and r/jobs threads
Search Reddit:
- `site:reddit.com "[Company Name]"`
- `site:reddit.com "[Company Name]" interview`
- `site:reddit.com "[Company Name]" recruiter`

Look for thread patterns: multiple unrelated users describing the same behavior, "I had the same thing happen" replies, specific bot or AI-interview reports.

## Verdict thresholds

| Signals fired | Verdict |
|---|---|
| 0-1 | Not enough evidence. Move on or hold for future sighting. |
| 2 | Add to `watchlist.md` with notes. Re-check on next sighting. |
| 3 or more | Add to `SkippedCompanies.md` and `SkippedCompanies.csv`. Skip the company on sight from now on. |

## Edge cases

- **Real legitimate firm in an adjacent space**: Don't auto-block just because a firm is a staffing agency or has India-based operations. Many legitimate IT staffing firms are headquartered in India. Look for the specific patterns above, not industry or geography alone.
- **Single bad recruiter at an otherwise legitimate firm**: Don't blocklist a multinational with thousands of recruiters because one bad seed sent spam. Look for systemic patterns.
- **Newly-registered domain that's actually new**: Recent registrations aren't always scams. Cross-check against age claims in marketing copy and other corroborating signals.

## What this list is NOT

This is not a defamation list. We aggregate publicly-reported patterns. We don't make original "X is a scam" claims. Read the sources we cite and decide for yourself.
