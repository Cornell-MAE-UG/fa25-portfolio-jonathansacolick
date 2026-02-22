
---
fontsize: 11pt
geometry: margin=1in
papersize: letter
pagestyle: empty
header-includes: \pagenumbering{gobble}
output: pdf_document
---

## Attacking Spotted Lanternflies' Reproduction Rate
**Team:** _Team Dragonfly_ **Clients:** Cornell CALS Extension / E\&J Gallo Winery / National Grape

**Problem Statement:**
Grape farmers in the Northeast US are invaded by spotted lanternflies (SLFs) that infiltrate harvests. The SLF population grows rapidly due to many nymphs surviving to adulthood, where they reproduce abundantly, increasing their population by a factor of 5.47. Current solutions primarily target adults, but rapid population growth is already occurring by this stage, increasing the severity of their impact regardless. 

**Impact:**
Decreasing SLF’s reproduction factor from 5.47 will slow down population increase and potentially stagnate it in an area, reducing the number of SLFs per vine from 400.

**Concept A (primary): SLF Scraper**

The Scraper would be a device that makes it quicker and simpler for SLF egg masses to be removed and allow for accessibility of egg masses in hard-to-reach places. The user would spot egg masses visually or using the light feature, extend the scraper using telescoping feature, and remove the egg masses off the surface to be dispensed into scraper housing. 

_Why it’s better than the status quo:_

- Current SLF scrapers are credit card-sized \& require close contact with the egg masses
- Our scraper makes the process simpler & improves overall accessibility

For our MVP, we will create a prototype that extends & contains egg masses and a preliminary UI. In the long term, we will create a working UI, camera system, and target reproducibility. 

**Concept B: Nymph Netting**

This involves weaving netting in a spiral formation to funnel and trap nymph SLFs that are unable to fly and climbing trees to feed, preventing them from reaching adulthood. This specifically targets nymphs and uses recent research to attract them by vibrating at a high frequency. 

**Key risks/Unknowns**

- Netting may unintentionally impact other wildlife, which would have negative ecological effects. We can reduce this by testing smaller scale traps with different entry funnels and setups.
- Even if the scraper is effective, without users consistently willing to use it, it will not impact the SLFs. To reduce this, we will create a survey to prioritize user input and improve our design based on their advice. 

**Questions**

1. **What are your biggest gripes with current scrapers used to remove egg masses?**  
   *Decision affected:* This will enable us to improve user comfort and efficiency. We can modify our scraper to match specific shapes or be more effective on certain textures if these are issues. 
2. **What traps are currently in use - how do they lure the SLFs, and are they effective?** 
   *Decision affected:* We can learn from these experiences to modify our traps (specifically the netting) to avoid ideas that do not work in practice.
3. **What are the main barriers to removing egg masses: are they too high to reach, too hard to scrape off due to geometry of the object, or a difficult consistency?**  
   *Decision affected:* Knowing this will allow us to design the geometry of the scraper for as many situations as possible and inform what features to focus on. 

\newpage

### References

- https://cals.cornell.edu/integrated-pest-management/outreach-education/whats-bugging-you/spotted-lanternfly/spotted-lanternfly-reported-distribution-map
- https://pubmed.ncbi.nlm.nih.gov/34302819/
- https://cals.cornell.edu/integrated-pest-management/outreach-education/whats-bugging-you/spotted-lanternfly/spotted-lanternfly-damage
