# BBL 2026 Final — Post-Match Analysis
**Sydney Sixers vs Sydney Thunder**

A delivery-level post-match analysis of the BBL 2026 Final, built from manually coded ball-by-ball data. The project produces coaching-grade insights supported by custom beehive and wagon wheel visualisations.

---

## Project Structure
bbl-2026-analysis/
├── data/
│   └── bbl_2026_final_coded.csv        # Ball-by-ball match data (239 deliveries, 28 variables)
├── bbl_2026_analysis.ipynb             # Delivery-level analysis for all three insights
├── beehive_final.py                    # Beehive chart generator (Hadley, Babar)
├── wagon_wheel.py                      # Wagon wheel generator (Smith vs pace, Smith vs Sangha, Babar)
├── BBL_2026_Final_Report_v3.pdf        # Post-match report
└── README.md

---

## Data Collection

Every delivery of the match was manually coded ball by ball, capturing 28 variables per delivery including:

- Line, length, shot played
- Intended and actual direction
- Ball speed (km/h)
- Batter handedness
- Dismissal type, fielder, caught at position
- Beaten, edged, middled flags

---

## Methodology

Data was processed in Python using pandas. Visualisations were built from scratch including handedness mirroring, jitter, and boundary distance formulas for accurate spatial representation.

The report follows a strict insight-first structure — each finding is written as a coaching recommendation, supported by a visual, with a clear action at the end.

---

## Key Findings

1. **Smith vs pace vs Sangha** — Smith scored at SR 341 against right-arm pace but was held to SR 100 by Sangha's leg spin on a tight middle/off corridor. Spin should have been introduced earlier.

2. **Hadley's length problem** — Hadley bowled good length outside off to Smith eight times without adjusting, conceding 26 runs from one zone. A mid-spell length change was the obvious fix.

3. **Babar Azam unchallenged** — Babar scored 47 off 39 largely because Thunder bowled width outside off throughout. Chris Green held him to SR 80 with a middle-stump line but no other bowler replicated it.

---

## Next Steps

Coding multiple matches across the BBL and Sheffield Shield seasons to move from single-game observations to cross-match patterns. One match tells you what happened. Multiple matches tell you why it keeps happening.

---

## Tools

- Python (pandas, matplotlib, numpy)
- Manual ball-by-ball coding in Google Sheets
- Node.js (docx) for report generation
