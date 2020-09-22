Demo data for Tableau data science demonstrations
=================================================


COVID-19 geographical dynamics: the tale of three states
--------------------------------------------------------

![COVID-19 use case screenshot](https://github.com/starschema/tableau-ds-demos/raw/master/screenshots/covid-19.png)

This demo showcases

* spatio-temporal splitting of a case-incidence time series, 
* comparing a timespan average versus a rolling comparison of the preceding time segment (use the date range slider to set the index date, and the choropleth will indicate % change in TPR against the preceding 14-day window), and
* trend lines.

There's a [detailed Wiki entry](https://github.com/starschema/tableau-ds-demos/wiki/COVID-19:-a-tale-of-three-states) that explains the narrative behind this use case.


Spatial analysis of fatal drug poisonings, 1998-2016
----------------------------------------------------

![Geospatial use case screenshot](https://github.com/starschema/tableau-ds-demos/raw/master/screenshots/geospatial-analytics.png)

This demo showcases

* spatial patterns: visualising spatiotemporal incidence patterns at a granular geographical level (US counties and the Federal District),
* time series trend detection: hovering over the individual counties shows the sparkline for the given county, and
* time series forecasting: shows a forecast at the 'tail' of established data, with an ambit of uncertainty (95% CI) based on a GLM.


Time series forecasting
-----------------------

![Time series use case](https://github.com/starschema/tableau-ds-demos/raw/master/screenshots/time-series-forecasting.png)

This demo uses the data set on the global average temperature deviation in degrees Celsius to showcase predictive capabilities, in particular

* using an external time series prediction (using `Prophet` in Python),
* displaying actuals (blue), predicted (orange) and 95% CIs (green and teal, respectively), and
* the integration of seasonality (from monthly data) into the forecast.


Survival
--------

![Survival use case](https://github.com/starschema/tableau-ds-demos/raw/master/screenshots/survival.png)

Typically, survival is visualised using the stepwise cumulative visualization. This is not always a useful way to see subcohort patterns. This use case utilises the data set by [Haberman et al.](https://archive.ics.uci.edu/ml/datasets/Haberman%27s+Survival) to display what fraction of individuals who had surgery for breast cancer in a given year survived or did not survive past the 5-year post-diagnostic interval, stratified by their age at the time of surgery. This use case displays

* a more intelligible way of identifying survival in cohorts, and
* a way to compare how survival changes (or rather, it doesn't: the majority of cases, in the 40-49 and 50-59 cohort, have relatively little change in survival, although as time goes on, survival of the 70-79 cohort did experience a significant survival benefit).
