# NYC Building Energy Efficiency Grades

![Add image here]()

This is the repository for the [NYC Open Data Week 2022](https://www.open-data.nyc/) workshop in which we analyze and map New York City's building energy efficiency grades with Python, Pandas, Geopandas, and Altair. This workshop was given on March 7, 2022 by [Juan Francisco Saldarriaga](https://brown.columbia.edu/portfolio/juan-francisco-saldarriaga-2/) from the [Brown Institute for Media Innovation](https://brown.columbia.edu/) at Columbia University's Journalism School.

## Data

The base files, provided by New York City's Department of Buildings, can be found in the [`input`](https://github.com/juanfrans/building-energy-grades/tree/main/input) folder. The Jupyter notebook analyzing the data can be found in the [`src`](https://github.com/juanfrans/building-energy-grades/tree/main/src) folder and the outputs from that analysis can be found in the [`output`](https://github.com/juanfrans/building-energy-grades/tree/main/output) folder.

A general explanation of the energy efficiency grading law, as well as a specific description of each energy efficiency grade can be found [here](https://www1.nyc.gov/site/buildings/codes/benchmarking.page).

After a FOIA request was submitted, NYC's Department of Buildings provided the following files:

* 2020 energy efficiency grades (in list form): `ll33_Data_Disclosure_2019-CBL.pdf`
* 2021 **preliminary** energy efficiency grades (in list form): `Preliminary\ 2021\ LL33\ Data\ Disclosure.xlsx`

Please read carefully this explanatory note from the Department of Buildings:

> Please note, the 2021 grades are considered “initial”, because the Department is currently in the process of reviewing benchmark report challenges and resubmittals from covered building owners for their 2021 grades. If a building owner files a successful challenge, that may result in a change of their 2021 letter grade. The full list of 2021 grades have not yet been posted on our website in a list or map form yet as they are not final.

The Department of Buildings also makes energy efficiency grade data available as an [interactive map](https://www1.nyc.gov/assets/sustainablebuildings/html/LL97-n-LL33-map.html). To view it click on the `LL33 | Energy Grades` tab at the top.

From that site we downloaded the 2020 energy efficiency grades as a shapefile: `ll33_2020.zip`.

## Event Description

We've all seen the energy grades posted at the entrances of large buildings in New York City. But how one building compare to its neighbor, or to buildings in other parts of the city? And how is the city doing overall? Are grades improving from year to year? Do newer buildings outperform older ones? Are there any interesting stories buried in the data?

This workshop will teach you mapmaking through programming — Python will be our language of choice, and we will introduce powerful packages like Pandas, Geopandas and Altair to explore geographic data. Our final product will be a Colab Notebook (similar to a Jupyter Notebook) with maps and graphs exploring the distribution of energy grades from 2020 and 2021 across the city and highlighting specific investigative leads.

This session will be led by [Juan Francisco Saldarriaga](https://brown.columbia.edu/portfolio/juan-francisco-saldarriaga-2/), Senior Data & Design Researcher at the [Brown Institute for Media Innovation](https://brown.columbia.edu/) at Columbia University's School of Journalism.

No prior programming experience is required.

## Plan

### Introduction

* Python, Colab, Geopandas, Altair
  * Why we do this this way instead of QGIS or ArcGIS
* Introduce the data
  * How we got it
  * What it was meant to do
    * Law
    * Press articles
    * Who is producing it and how
  * What are the files that we will be using
  * Where is the data
    * Why in Github?
* What is the plan today
  * Explore
  * Produce initial visualizations

### Analysis

* Loading libraries
  * Why libraries?
  * Which ones
* Loading data
  * Different types of data
  * Head, tail, describe, info, dtypes, sample
  * Summary statistics
    * Max, median, mean, std, min
  * Graphs
* Group by
  * Borough
  * Graphs
* What buildings changed the most?
* Bring in nta data
  * Merge
  * Does it need to happen at the centroid level
  * Map
* Bring in PLUTO
  * Type of building
    * Building class
    * Area
    * Number of units