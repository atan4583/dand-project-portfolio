# Prosper Loan Dataset Exploration

## Dataset
The data consists of 6,123 Prosper loan listings created between 1 July 2008 and 31 December 2009 from Prosper, an online peer-to-peer lending business. The data has 16 features
(excluding two ID type variables for borrower ID and listing key), most of which are quantitative in nature but there are a few categorical ones as well.

A data feature dictionary describing the variables is available [here](https://www.google.com/url?q=https://docs.google.com/spreadsheet/ccc?key%3D0AllIqIyvWZdadDd5NTlqZ1pBMHlsUjdrOTZHaVBuSlE%26usp%3Dsharing&sa=D&ust=1554484977407000).

The dataset for _**exploration**_ can be downloaded [here](https://drive.google.com/file/d/1SSRs1cna9JoYpQg0sox1d9swT01GEacR/view?usp=sharing), and the clean dataset for _**explanatory**_ purpose can be downloaded [here](https://drive.google.com/file/d/1WSURY1r0B4xh5RVV9asR473hxbGAePM-/view?usp=sharing).


## Summary of Findings
In the exploration, we focused on 6,123 listings between 1 July 2008 and 31 December 2009, and examined selective attributes on borrower and loans, time series events to see their effects on loan listing distributions.

In univariate exploration, we found:
-  distributions of listing categories, borrower professions and states tell us majority of listings were for debt consolidation, most of the borrowers held professional jobs and residents of CA had the highest number of listings.


- distribution listing amount shows majority of loan listings were below $3000 in values, employment status distribution shows a combined 97.02% of borrowers were in full, self or part time employment statuses. Yet listings in charged off and defaulted statuses is significant at 26.14% combined.

In bivariate exploration, we observed that listing amount distribution is concentrated in lower end of loan values, well below $10,000. This is consistent with our finding in univariate exploration. We also see that adding a second feature to previously explored features can cause distribution trends to vary, as seen here in the two scenarios where _**Occupation**_ and _**Credit**_ Ranking were added in turn to listing distribution in the top five borrower states. In both cases, the listing distributions vary from their corresponding distributions in univariate exploration.

In multivariate exploration, we learned adding a related new feature to a bivariate distribution does result in the related features strengthening each other. For examples,
- adding a third feature _**Borrower APR**_ to the bivariate distribution of listing amount and credit ranking adds visibility to varying concentrations of listing amounts at different APR rates.


- adding a fourth feature _**Listing Category**_ to multivariate distribution of listing amount and borrower APR by credit ranking enables visibility to segmentation of borrower APR on listing amount and credit ranking by listing category.


- the three features _**Time**_, _**Principal borrowed**_ and _**Delinquent amount**_ enhance each other and yield a clear trend on principal borrowed and linquent amount between 1 July 2008 and 31 December 2009.


- the three features _**Listing amount**_, _**Credit ranking**_ and _**Period**_ enhance each other and enable comparison of listing amount and credit ranking distribution in two different time periods.


- the three feature _**Listing amount**_, _**Listing category**_ and _**Period**_ enhance each other and add visibility to listing amount and listing category distribution in two different time periods.

Through univariate, bivariate and multivariate explorations, we were able to look at features pertaining to Prosper borrowers, loan listings and time periods in the dataset to study their influences on Prosper loan distributions, and see the effect of the three historical significant events on Prosper loan listings between 1 July 2008 and 31 December 2009.

## Key Insights for Presentation
For the presentation, we focus on showing the effects of selective borrower, loan attributes and time series events on Prosper loan listing distributions.

We start with introducing visuals of listing distributions associated with borrower profession, employment status, resident state, listing category, listing status and listing amount in univariate perspective.

Next, we demonstrate how adding an additional attribute to univariate listing distributions can result in variations in listing distributions.

Lastly, we create multivariate visuals by adding APR and time series attributes to bivariate listing distributions, show casing the effects of these attributes on multivariate listing distributions.          

---
## Acknowledgement
Special thanks to the _**legendary**_ Udacity Data Analyst Nanodegree mentor _**Myles Callan**_, whose knowledge competency is impressively splendid, and dedication to serve students, undeniably unparalleled. I have benefited and learned a great deal from his remarkble style of coaching.

Thank you, _**Myles**_, for the privilege to learn from you, you are simply wonderful !!!

---
## References

### Udacity Data Visualization
[Lesson 3-4 : Absolute vs Relative Frequency](https://youtu.be/FpnZ7dH4FqU)

[Lesson 4-9 : Clustered Bar Charts](https://youtu.be/0rFp55TtEJM)

[Lesson 4-11 : Faceting](https://youtu.be/oUYRqI6wFGw)

[Lesson 5-2 : Non-Postional Encodings for Third Variables](https://youtu.be/D91mm-qaDkk)

[Lesson 5-3 : Color Palettes](https://youtu.be/nirOTWkuiSM)

[Lesson 5-5 : Faceting in Two Directions](https://youtu.be/lz5dcoTcV2o)

[Lesson 6-8 : Creating a Slide Deck with Jupyter](https://youtu.be/qIot9qrvcF8)


### Miscellaneous Online References
[How to Pick the Perfect Color Combination for Your Data Visualization](https://blog.hubspot.com/marketing/color-combination-data-visualization)

[Matplotlib cmap reference](https://matplotlib.org/gallery/color/colormap_reference.html)

[Scatterplot with hue](https://python-graph-gallery.com/43-use-categorical-variable-to-color-scatterplot-seaborn/)

[Ticklabel formatter](https://stackoverflow.com/questions/53747298/how-to-format-seaborn-matplotlib-axis-tick-labels-from-number-to-thousands-or-mi)

[How to specify legend position in matplotlib in graph coordinates](https://stackoverflow.com/questions/44413020/how-to-specify-legend-position-in-matplotlib-in-graph-coordinates)

[Time Series Data Visualization with Python](https://machinelearningmastery.com/time-series-data-visualization-with-python/)

[Color tutorial](https://www.codecademy.com/articles/seaborn-design-ii)
