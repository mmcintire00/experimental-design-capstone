## Experimental Design Capstone
### Project: Analysis of Gulf of Mexico lease sale bids

### Background: The Gulf of Mexico (GOM) is considered one of the most prolific oil and gas basins in the world. The basin has produced to date more than 5.2 Billion Barrels of Oil Equivalent (BBOE). The GOM is divided into protraction areas and these protraction areas are further broken into 3 mile by 3 mile lease blocks. The blocks are controled the Beauru of Ocean and Energy Managment. Oil and gas companies with a license to operate in the GOM can bid on available leases in yearly lease sales. Lease terms vary from 5-10 years depending on water depth.

### One of the primary jobs of the subsurface staff at an oil and gas company is to monitor competitor lease aquisition. A company's leasing history can show where a that company, or the industry as a whole, are focusing money and exploration efforts. Competitor intelligence can also help companies create their own strategies for leasing, building exploration campaigns, or provide justification to drill a well. It's important to remember that the lease boudries created by the federal government do not control the geology in the subsurface. Oil and gas fields frequently cross lease boundries, so understanding what targets companies around your own leases and infrastructure are pursuing can help protect your own reserves and identify potential targets for joint ventures and future exploration. The key audience for this project are subsurface staff (geoscientists and reservoir engineers), middle management, and executives at oil and gas companies that opporate in the Gulf of Mexico.

### Project Question: Is using mean lease sale bids per year a good indicator of a company’s commitment to exploration?

### Hypothesis:

* Ho: There is no significant difference in the mean bid (USD) per lease block per company between 2014-2020.
* Ha: There is a significant difference in the mean bid (USD) per lease block per company between 2014-2020

### Data: The data is publicly available on the BOEM website. The dataset contains 1708 records and 17 variables. I've only imported 10 variables to be used for this analysis. There are no missing values.

### Discussion and Conclusions:

* After performing the one way ANOVA test the p-value is .499, which is greater than .05. We can assume that the means being compared are similar. When looking at the line plots of the mean bids over the given time frame, the mean values plot similarly. 

* This dataset is interesting beause it captures two major oil price collapses (2015 & 2020). The means may be similar form 2015-2020 because companies became more disciplined in spending in order to conserve money during the downturns. The lease sale in 2014 shows a larger amount and distribution of lease bids submitted possibly due to high oil prices.

### Future Work:

*   Comparing median to account for outlier bids. Should we think about these bids similar to the homeprices example? One really high bid is not an invalid point. Quickly tested this in the above section. comparing mean bid to median bid. 
*   Comparing bid count per company and per area between 2014-2020. This might show emerging exploration areas better than mean bid amount. See below!
*   adding average oil price per year to main dataframe
*   scraping budgets from companies to compare
*   comparing average stock price for publicly traded companies with mean bid or # of bids
*   permits for exploration wells filed by company 
*   total volumes produced per company to measure exploration success
*   number of leases available vs num bids submitted

### Possible bias:
*   sampling bias: In order to complete a more thorough test I needed eliminate companies that did not participate in all 7 years of lease sales. Some of the companies I had to remove were private equity firms that may not have been constrained by a budget scrutinized by the investment community. Could I change null values to zero and rerun analysis?
*   contextual bias: The big one is likely the effect of oil price, which would cause budgets to tighten and making companies less likely to spend more money on lease bids.






