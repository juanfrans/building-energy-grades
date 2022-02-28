# NYC Building Energy Efficiency Grades

![Add image here]()

This is the repository for the [NYC Open Data Week 2022](https://www.open-data.nyc/) workshop in which we analyze and map New York City's building energy efficiency grades with Python, Pandas, Geopandas, and Altair. This workshop was given on March 7, 2022 by [Juan Francisco Saldarriaga](https://brown.columbia.edu/portfolio/juan-francisco-saldarriaga-2/) from the [Brown Institute for Media Innovation](https://brown.columbia.edu/) at Columbia University's Journalism School.

The base files, provided by New York City's Department of Buildings, can be found in the `input` folder. The Jupyter notebook analyzing the data can be found in the `src` folder and the outputs from that analysis can be found in the `output` folder.

A general explanation of the energy efficiency grading law, as well as a specific description of each energy efficiency grade can be found [here](https://www1.nyc.gov/site/buildings/codes/benchmarking.page).

After a FOIA request was submitted, NYC's Department of Buildings provided the following files:

* 2020 energy efficiency grades (in list form): `ll33_Data_Disclosure_2019-CBL.pdf`
* 2021 **preliminary** energy efficiency grades (in list form): `Preliminary\ 2021\ LL33\ Data\ Disclosure.xlsx`

Please take into account the this explanatory note by the Department of Buildings:

> Please note, the 2021 grades are considered “initial”, because the Department is currently in the process of reviewing benchmark report challenges and resubmittals from covered building owners for their 2021 grades. If a building owner files a successful challenge, that may result in a change of their 2021 letter grade. The full list of 2021 grades have not yet been posted on our website in a list or map form yet as they are not final.

The Department of Buildings also makes energy efficiency grade data available as an [interactive map](https://www1.nyc.gov/assets/sustainablebuildings/html/LL97-n-LL33-map.html). To view it click on the `LL33 | Energy Grades` tab at the top.

From that site we downloaded the 2020 energy efficiency grades as a shapefile: `ll33_2020.zip`.