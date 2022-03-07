# Visualising areas of London

This repository contains the source code for a JavaScript visualisation of crime rates, scenicness and indices of deprivation across London. This is the standalone code associated with the visualisation presented [here](https://github.com/wrattler/wrattler-examples/blob/master/examples/scenic-analysis.wrattler), where further quantitative analysis of the data can be found.

It presents the following data sources:

- **Crime data** - average total number of crimes per month in Lower Super Output Area (LSOA) geographic locations in London obtained from the Government, [MPS LSOA Level Crime (historic)](https://data.london.gov.uk/dataset/recorded_crime_summary).

- **Indices of deprivation and population density** - indicators of deprivation relating to health, employment, housing, income rate, living environment, and education obtained from the Government [here](https://data.london.gov.uk/dataset/indices-of-deprivation) (see 'IMDB2015' sheet in .xls) and [here](https://data.london.gov.uk/dataset/lsoa-atlas). A higher level of deprivation relating to health, employment, income rate, education and living environment, is indicated by emptier bars in the top left panel of the visualisation.

- **Scenic ratings** - measures of scenicness of an area given by a neural network, specifically, a CNN that was trained on Scenic-Or-Not data. The Scenic-Or-Not dataset contains around 217,000 images of landscapes that cover nearly 95% of the UK - and has 1.5 million ratings of scenicness from members of the public and counting. In order to improve the performance for Google Street View images, this CNN was further trained on the 6,946 Google Street View images. The full method has been discussed by [Law et al. (2018)](https://www.tandfonline.com/doi/abs/10.1080/13658816.2018.1555832).

</br>
<p align="center"><img src="docs/scenicness.png" width="800"></p>
</br>
<p align="center"><img src="docs/scenic_points.png" width="800"></p>
</br>
<p align="center"><img src="docs/mean_counts.png" width="800"></p>

## Built With

- [Leaflet](https://leafletjs.com/)
- [D3](https://d3js.org/)
- [jQuery](https://jquery.com/)
