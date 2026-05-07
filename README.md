# Left Behind and Moving Right: Do Deprived Regions Predict Authoritarian Personalities?

**Lewis Sydney Campbell Hall · POLI3148 · halll22@cardiff.ac.uk**

---

## Overview

Within Europe, urban centres drive economies, leaving a growing number of regions 'left-behind' as the OECD labels. This project investigates whether regional deprivation predicts the emergence of right-wing authoritarian personality tendencies among residents, moving beyond material dimensions of previous literature to explore psychological dimensions also.

The (right-wing) authoritarian personality theorised by Altemeyer (1996) is modelled through its three core tendencies: submission to authority, aggression to others, and adherence to tradition. The central argument is that deprivation causes authoritarian tendencies both directly and indirectly (through decline in personal and institutional trust).

France's *diagonale du vide*, is the primary case study, given its OECD designation as a consistent left-behind corridor and its documented right-wing voting patterns.

---

## Repository Structure

Code and data are organised across **branches**; all figures and visualisations are available within code in the 🔗 **[index page](https://lewishall05-pixel.github.io/deprived_regions_and_authoritarian_personalities/)**.


| Branch | Contents |
|--------|----------|
| `main` | README |
| `code` | Google Colab (Python) notebooks |
| `data` | ESS datasets in ZIP files |
| `docs` | HTML webpage of code |

---

## Research Question

Do left-behind regions cause higher authoritarian personality scores, therefore increasing right-authoritarian vote share?

---

## Data & Methodology

- Primary dataset: European Social Survey Round 11 (2023/4), 50,116 respondents, 30 countries
- Authoritarian Personality Index: constructed from 9 ESS variables across the three dimensions of submission, aggression, and adherence.
- Left-Behind Score: derived from GDP relative to the EU28 mean, combined with growth trajectory (OECD method)
- Causal identification: lagged predictors (2015 Left-Behind Score → 2023/4 Authoritarian Index); mediation analysis via trust indicators (*Trust in Others*, *Trust in Legislatures*, *Trust in Parliament*, *Economic Satisfaction*)
- Fixed effects: two-way fixed effects across ESS Rounds 6–11 to distinguish intranational from international variation

---

## Key Findings

- The 2015 left-behind score significantly predicts higher 2023/4 authoritarian personality scores (β = 0.0388, p = 0.00 lagged; β = 0.0454, p = 0.00 concurrent); raw and control regressions are positive.
- 33.8% of the relationship is mediated through trust — deprivation lowers institutional and personal trust, which in turn reinforces authoritarian attitudes. The direct path remains significant, indicating partial mediation.
- Two-way fixed effects show that intranational left-behind differences better predict authoritarian tendency than international differences — voter behaviour is final stage in a path of economic decline → trust decline → authoritarian incline.
- In the *diagonale du vide* case study, both authoritarian attitude scores and *Rassemblement National* vote share track closely along the left-behind line, evidencing the deprivation → attitude → vote path.

---
## Replicating the Results

All materials needed to replicate analysis are available in the repository on branches:
- **`data`** 
- **`code`**

### Steps

1. Clone the repository with the branches.

2. Get the data - no external downloads required, all processed ESS11-ESS8 data is included.

3. Install required Python packages.

4. Run code notebook cells in order.

---

*University of Hong Kong*
