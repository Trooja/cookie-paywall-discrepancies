# Repository for the results from the thesis Assessing discrepancies in cross-browser paywalls detection.

This repository contains the aggregated results from the thesis Assessing discrepancies in cross-browser paywalls detection performed by Andreas Stenwreth and Simon Täng at Chalmers University of Technology from March until August 2024. 

The following files are included:

### all-paywalls.csv
This file contains the 804 websites used in the thesis that presented cookie paywalls on June 3, 2024, when accessed using Chrome on Linux from Sweden. 
For each website, this file contains:

- country  - the country in which the domain is registered.
- category - the type of website and content it - contains e.g News. 
- smp      - the Subscription Management Platform used (either Contentpass or Freechoice)
- cmp      - the Consent Management Platform used.

### double-paywalls.csv
This file contains a subset of all studied websites, which, in addition to presenting a cookie paywall present a hard or soft paywall in order to prevent access to content on the website.
For each website, this file contains:

- country  - the country in which the domain is registered.
- category - the type of website and content it contains e.g News. 
- smp      - the Subscription Management Platform used (either Contentpass or Freechoice)
- cmp      - the Consent Management Platform used.

### no-paywalls.csv
This file contains 200 websites that were manually verified to not present a cookie paywall when accessed from Chorme on Linux from Sweden on June 19, 2024. 

### validation.csv
This file contains a random subset of all studied websites used for manual inspection. Manual inspection was performed by comparing the developed crawler program output with the screenshot taken during the crawl for each website and combination of web browser, operating system, and geocraphic location. 
For each website, this file contains:

- ok   - 1 if the output and screenshot are consistent for all combinations; otherwise, 0.
- note - if not, the note outlines which combinations were incorrect. 

# Software

Software used was [Selenium](https://www.selenium.dev/documentation/) and [Selenium Grid](https://www.selenium.dev/documentation/grid/) version 4.21 and [Appium](https://appium.io/docs/en/latest/#) version 2.9.

The following list includes all operating systems and web browsers used during the thesis. 
All browsers ran in their respective privacy modes, allowing all third-party cookies.

- **Linux: Debian GNU/Linux 12 (bookworm)**
    - Firefox 115.12.0esr
    - Chrome 126.0.6478.55
    - Edge  125.0.2535.92
- **Windows: 11 Home 23H2**
    - Firefox 127.0
    - Chrome 126.0.6478.62
    - Edge  126.0.2592.56
- **MacOS: Sonoma Version 14.5**
    - Firefox 127.0
    - Chrome 125.0.6422.142
    - Edge 126.0.2592.56
    - Safari 17.5
- **IOS: 17.5**
    - Safari 17.5
- **Android: 10 52.1.A.3.137**
    - Firefox 127.0
    - Chrome 126.0.6478.55


