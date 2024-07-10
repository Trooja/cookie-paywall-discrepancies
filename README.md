# Repository for the results from thesis Assessing discrepancies in cross-browser paywalls detection.

This repository contains the aggregated results form the thesis Assessing discrepancies in cross-browser paywalls detection performed by Andreas Stenwreth and Simon Tang at Chalmers University of Technology from Mars until August 2024. 

The following files are included:

### all-paywalls.csv
This file contain the 804 websites used in the thesis that presented a cookie paywalls on June 3 2024 when accessed using Chrome on Linux from Sweden. 
For each website this file contain:

- country  - the country in which the domain is registered.
- category - the type of website and content it - contains e.g News. 
- smp      - the Subscription Management Platform used (either Contentpass or Freechoice)
- cmp      - the Consent Management Platform used.

### double-paywalls.csv
This file contain a subset of all studied websites which which in addition to presenting a cookie paywall also present a hard or soft paywall in order to access all content on the website.
For each website this file contain:

- country  - the country in which the domain is registered.
- category - the type of website and content it contains e.g News. 
- smp      - the Subscription Management Platform used (either Contentpass or Freechoice)
- cmp      - the Consent Management Platform used.


### validation.csv
This file contain a random subset of all studied websites used for manual inspection. Manual inspection was performed by comparing the developed crawler programs output with the screenshot taken during the crawl for each website and combination of web browser, operating system and geocraphic location. 
For each website this file contain:

- ok   - 1 if the output and screenshot is consistent for of all combinations else 0.
- note - if not ok, the note outlines which combinations were incorrect. 
