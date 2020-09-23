Demo data for Tableau data science demonstrations
=================================================


Drug performance mining
-----------------------

![Drug performance mining](https://github.com/starschema/tableau-ds-demos/raw/master/screenshots/regression.png)

This demo showcases Tableau's new regression modelling capabilities by identifying whether a particular medication performs above or below the expected value based on how patients rate the drug. Consider, for instance, this comparison of duloxetine (Cymbalta) and mirtazapine:

![Drug performance mining](https://github.com/starschema/tableau-ds-demos/raw/master/screenshots/duloxetine_vs_mirtazapine.png)

Both drugs have roughly the same number of users. However, Cymbalta is rated quite lower than mirtazapine, thus in relation to each other, Cymbalta is a better performer than mirtazapine.


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

![Time series use case screenshot](https://github.com/starschema/tableau-ds-demos/raw/master/screenshots/time-series-forecasting.png)

This demo uses the data set on the global average temperature deviation in degrees Celsius to showcase predictive capabilities, in particular

* using an external time series prediction (using `Prophet` in Python),
* displaying actuals (blue), predicted (orange) and 95% CIs (green and teal, respectively), and
* the integration of seasonality (from monthly data) into the forecast.


Reliability and adverse events
------------------------------

![Reliability screenshot](https://github.com/starschema/tableau-ds-demos/raw/master/screenshots/reliability.png)

This demo shows anomaly detection capabilities on the illustration of a (fictional!) data set simulating five side effects of a drug in three common patterns: constant-rate, constantly increasing rate and accumulative effects, where a previously unidentifiable part of the treatment cohort who are so susceptible exhibit the side effect after a given time in treatment. This illustrates

* using Tableau to identify anomalies, and
* using rolling calculations to identify the rapid spike in encephalopathy, isolated in time.


Survival
--------

![Survival use case screenshot](https://github.com/starschema/tableau-ds-demos/raw/master/screenshots/survival.png)

Typically, survival is visualised using the stepwise cumulative visualization. This is not always a useful way to see subcohort patterns. This use case utilises the data set by [Haberman et al.](https://archive.ics.uci.edu/ml/datasets/Haberman%27s+Survival) to display what fraction of individuals who had surgery for breast cancer in a given year survived or did not survive past the 5-year post-diagnostic interval, stratified by their age at the time of surgery. This use case displays

* a more intelligible way of identifying survival in cohorts, and
* a way to compare how survival changes (or rather, it doesn't: the majority of cases, in the 40-49 and 50-59 cohort, have relatively little change in survival, although as time goes on, survival of the 70-79 cohort did experience a significant survival benefit).
