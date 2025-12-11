## Predicting the Severity of Major Power Outages in the U.S.

## Introduction
Power outages disrupt millions of lives, which raises pressing issues like public safety and emergence response to economic stability. A power outage may seem like a simple inconvenience, like losing the chance to finish a show on Netflix, but its real impact goes far beyond that. In severe situations a power outage can  disable critical medical equipment, shut down heating or cooling during extreme weather, interrupt communication systems used by first responders, halt transportation services, and cause widespread economic losses for businesses and communities. Summary statistics of some variables which intuitively contribute most to the power outage are shown below.

To better understand these events, this project uses the Major Power Outage Events dataset which records 1,535 power outages occurring in the United States. Each outage has around 57 categories of information. This wide range of information makes us wonder about the severity of the power outages. Hence this project will explore the central question of What factors influence how long a major power outage lasts, and can we predict outage duration using the available data? This prediction problem will be useful for policymakers and the general community to according plan for the outage according to its severity. This will help them to allocate resources, and prepare for emergency needs.


## Data Cleaning and Exploratory Data Analysis
<iframe
  src="assets/univariate_analysis_cause.category.html"
  width="800"
  height="600"
  frameborder="0"
></iframe>

<iframe
  src="assets/univariate_analysis_climate.region.html"
  width="800"
  height="600"
  frameborder="0"
></iframe>

<iframe
  src="assets/bivariate_analysis_cause.category_vs_dur_hours_box_plot.html"
  width="800"
  height="600"
  frameborder="0"
></iframe>

<iframe
  src="assets/map.html"
  width="800"
  height="600"
  frameborder="0"
></iframe>

## Assessment of Missingness
Based on the dataset the column which is most likely to be **NMAR** (Not Missing at Random) is
`demand.loss (megawatt)` During large severe outages, reporting systems are often deprioritized which increases the likelihood that the larger (unobserved) values of outages are missing. This further means that missing may be directly related to the variable itself (the definition of NMAR).
To frame it as **MAR** (Missing at Random) further information on why the values are missing would be needed. This additional information could be wind speed, precipitation, some disaster report or reporting system failure is needed. If these factors can convey some correlation with the missingness in demand.loss (megawatt) then MAR can be justified. 

## Hypothesis Testing
<iframe
  src="assets/kde_is_normal_climate_True_False_dur_hours.html"
  width="800"
  height="600"
  frameborder="0"
></iframe>

## Framing a Prediction Problem

## Baseline Model

## Final Model

## Fairness Analysis
