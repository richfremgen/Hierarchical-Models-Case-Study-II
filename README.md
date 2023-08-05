# Hierarchical-Models-Case-Study-II
Using a Bayesian Hierarchical Model to analyze North Carolina voter registration data

## Analysis

### Introduction
You have been contracted by a political campaign to analyze voter registration data in North Carolina. The North Carolina State Board of Elections (NCSBE) is the agency charged with the administration of the elections process and campaign finance disclosure and compliance. Among other things, they provide voter registration and turnout data online. The Census Bureau is the principal agency of the U.S. Federal Statistical System, responsible for compiling and disseminating data about the American peopple. Their data is available online here. Using the NC voter files for the general 2016 election, as well as the census reports for NC in 2010, you will attempt to estimate how different demographic groups registered to vote in 2016.

### Data
The dataset `voter_stats_20161108.txt` contains information about the aggregate counts of registered voters by the demographic variables. The provided variables in this dataset are:

* `county_desc` : Description of the county
* `election_date` : Date of the election
* `stats_type` : Voter or not
* `precinct_abbrv` : Precincts: the lowest-level of grouping for a city, town or county. The county commission divides the county into precincts for the purpose of voting. A precinct must have visible, definable and observable physical boundaries that conform to standards set by the U.S. Bureau of the Census for defining census blocks for their census.
* `vtd_abbrv` : Voting districts as defined by the US Census to include the wide variety of small polling areas, such as election districts, precincts, or wards, that State and local governments create for the purpose of administering elections. The voting districts are not strictly equal to the precincts so that multiple precincts can map to the same voting district.
* `party_cd` : Party of the candidate
* `race_code` : Race of the group
* `ethnic_code` : Hispanic origin of the group
* `sex_code` : Gender of the group
* `age` : Age groups
* `total_voters` : Total number of registered voters within groups

You will need to use both of these to adequately answer the questions of interest. Whether or how you choose to merge the datasets is up to you. Moreover, the entire dataset is too large to conveniently work with. You will only work with a subset of the overall data. Take a random sample of 30 counties out of all the counties in both datasets. You should indicate the counties you sampled in your final report.

## Questions of interest

Your job is to use a Bayesian hierarchical model to answer the following questions of interest. 

* How did different demographic subgroups register to vote in the 2016 elections?
* For example, how did the registration rate for males compare to the registration rate for females after controlling for other potential predictors? Did the overall probability or odds of registering to vote differ by county in 2016?
* Which counties differ the most from other counties?
* How did the registration rates differ between females and males for the different party affiliations?
* How did the registration rates differ between age groups for the different party affiliations?

Be sure to include the following in your report:

The final models you ultimately decided to use, clear model building, that is, justification for the models (e.g., why you chose certain transformations and 
why you decided the final models are reasonable), model assessment and validation for the final models (think residual binned plots, accuracy, AUC, etc), the relevant model outputs (table of coefficients with SEs and/or confidence intervals, etc), your interpretation of the results in the context of the questions of interest, including clear and direct answers to the questions posed, and any potential limitations of the analyses.
