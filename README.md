Data Analysis Projects — Justin Gao
UW Informatics · Data Science Track
A collection of data analysis projects from my coursework at the University of Washington, built in R using tidyverse, ggplot2, and Quarto.

COVID-19 Impact on Seattle Property Values
Course: INFO 201 — Technical Foundations of Informatics
Tools: R, tidyverse, ggplot2, Quarto (revealjs)
Data: FHFA House Price Index (FRED) · Seattle Building Permits (City of Seattle Open Data Portal)
Overview
Analyzed how the COVID-19 pandemic affected residential property values and construction activity in Seattle using two public datasets spanning 2018–2025.
Key Questions

Did house prices increase or decrease during COVID?
How did quarterly price growth rates change across periods?
Did construction activity slow down?
Were single-family and multifamily housing affected differently?

Methods

Classified observations into Pre-COVID, During COVID, and Post-COVID periods using case_when() and date functions (ymd, year, quarter)
Computed quarterly growth rates with lag() and summarized averages by period using group_by + summarise
Joined house price and permit datasets by COVID period using inner_join to explore the relationship between prices and development activity

Findings

Seattle home prices jumped ~21% during COVID (2020–2021), compared to ~10% growth in the two years prior
Quarterly growth rates peaked during COVID at ~3.5% per quarter
Construction permit volume stayed relatively stable during COVID and increased post-pandemic
Multifamily project costs were volatile — dropping during COVID then surging post-pandemic — while single-family costs rose steadily
High prices during COVID did not immediately translate to more building activity

Visualizations

Line chart: House Price Index over time, colored by period
Box plot: Quarterly growth rate distributions by COVID period
Grouped bar chart: Permit counts and average project costs by housing type and period
Scatter plot: Average price index vs. total permits by period


Skills Demonstrated

Data wrangling with tidyverse (mutate, filter, group_by, summarise, arrange, inner_join)
Date parsing and period classification with lubridate
Data visualization with ggplot2
Reproducible reporting with Quarto
