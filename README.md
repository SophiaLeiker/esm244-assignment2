# ESM 244 Assignment 2

*** 

## Part 1

This report will employ binary logistic regression to test feasibility of using variables plant height (height), canopy length (length), canopy width (width), and number of green leaves (green_lvs) to classify whether a palmetto is species Serenoa repens or Sabal etonia.

The analysis will be performed twice, and will use cross validation to compare two models:

- Log odds of plant type using plant height, canopy length, canopy width and green leaves as predictor variable.
- Log odds of plant type using plant height, canopy width and green leaves (i.e., drop canopy length for this model)


**Data Source:** The data used comes from: [Abrahamson, W.G. 2019. Survival, growth and biomass estimates of two dominant palmetto species of south-central Florida from 1981 - 2017, ongoing at 5-year intervals ver 1. Environmental Data Initiative](https://doi.org/10.6073/pasta/f2f96ec76fbbd4b9db431c79a770c4d5) and metadata, including methods used for data collection can be found here [EDI Data Portal](https://portal.edirepository.org/nis/metadataviewer?packageid=edi.317.1).
The first dataset, palmetto_data, contains survival and growth data across multiple years, habitats and experimental treatments. The second dataset, seedlings_data, follows the fate of marked putative palmetto seedlings in the field to assess survivorship and growth. The final dataset, harvested_palmetto_data, contains size data and estimated dry mass (biomass in grams) of 33 destructively harvested palmetto plants (17 S. repens and 16 S. etonia) of varying sizes and across habitats.

***

### Part 2

This report will employ non linear least squares to estimate parameters of a length to weight model for lizard populations in New Mexico. To do this the  snout length to weight model will be used. 


**Data Source:** The data used comes from: [Lightfoot, D. and W.G. Whitford. 2020. Lizard pitfall trap data from 11 NPP study locations at the Jornada Basin LTER site, 1989-2006 ver 37. Environmental Data Initiative. ](https://doi.org/10.6073/pasta/4a6e258fb49c31e222ecbbcfd128967f) and metadata, including raw data and methods used for data collection can be found here [EDI Data Portal](https://portal.edirepository.org/nis/mapbrowse?packageid=knb-lter-jrn.210007001.37).

This data package contains data on lizards sampled by pitfall traps located at 11 consumer plots at Jornada Basin LTER site from 1989-2006. Lizards were captured in pitfall traps at the 11 LTER II/III consumer plots (a subset of NPP plots) quarterly for 2 weeks per quarter. Variables measured include species, sex, recapture status, snout-vent length, total length, weight, and whether tail is broken or whole.

- This report will fit an NLS model
- Providing our model with initial guesses
- Do OLS regression
- Supply nls start with regression coefficients
