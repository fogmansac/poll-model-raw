---
license: cc-by-sa-4.0
pretty_name: US 2026 Election Polls
tags:
- elections
- polls
- politics
- united-states
size_categories:
- 1K<n<10K
configs:
- config_name: default
  data_files: "data/*.csv"
---

# US 2026 Election Polls

Public opinion polls for the 2026 US midterm races (Senate, governor, House and generic ballot), the 2,000 most
recent, one row per poll and matchup. `results` is a JSON list of candidates with party and percentage.

| column | meaning |
|---|---|
| race, state, office, stage | the race polled |
| matchup | candidates in the question |
| pollster, sponsorPartisan | who ran it, and a partisan sponsor if any |
| startDate, endDate | fieldwork dates |
| sampleSize, population, marginOfError | sample (LV likely voters, RV registered, A adults) |
| results | JSON: candidate, party, pct |
| leader, leadMargin | who leads and by how many points |
| releaseDate, pollReleaseUrl | when and where the pollster released it, when known |
| sourceUrl | the Wikipedia page the poll was read from |

License: CC BY-SA 4.0. The poll tables come from Wikipedia's 2026 race articles; credit "Wikipedia contributors" and share
derivatives under the same license.

The same data, live and filterable, is available as an API: [Political Polls API](https://pushbuild.com/apis/political-polls.html).

Published by Pushbuild. Pushbuild is not affiliated with the data's original publishers.
