# Metadata

| Column No | Column Label                                      | Explanation                                                                                                             |
|-----------|---------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------|
| 1         | SampleID                                          | This column simply shows the 403 different watermelon sample identifiers compiled by Yang et al. (2022).                 |
| 2-62      | Chr01x343067xAxC, Chr01x148789xAxG, ...           | These columns represent genetic variants (SNPs) extracted from the watermelon samples which have high association with environmental variables. The delimiter 'x' is used for compatibility with HBase. The format is Chromosome:Position:Reference Allele:Alternate Allele (e.g., Chr01x343067xAxC means Chromosome 1, Position 343067, Reference Allele A, Alternate Allele C). |
| 63        | Location                                          | This column indicates the location where the samples are found. Prior to pre-processing before importing into HBase, this location corresponds to a latitude and longitude were used to extract the bioclimate variables and environmental variables from the latitude and longitude. The latitude and longitude is then dropped as the location may convey more meaningful insights for the HBase analysis later. |
| 64-82     | bioclim1 – Annual Mean Temperature                | These variables are extracted from bioclimate data. Every bioclimatic variable is indicated and explained in terms of its representativeness in the column on the left. |
|           | bioclim10 – Mean Temperature of Warmest Quarter   |                                                                                                                         |
|           | bioclim11 – Mean Temperature of Coldest Quarter   |                                                                                                                         |
|           | bioclim12 – Annual Precipitation                  |                                                                                                                         |
|           | bioclim13 – Precipitation of Wettest Month        |                                                                                                                         |
|           | bioclim14 – Precipitation of Driest Month         |                                                                                                                         |
|           | bioclim15 – Precipitation of Seasonality          |                                                                                                                         |
|           | bioclim16 – Precipitation of Wettest Quarter      |                                                                                                                         |
|           | bioclim17 – Precipitation of Driest Quarter       |                                                                                                                         |
|           | bioclim18 – Precipitation of Warmest Quarter      |                                                                                                                         |
|           | bioclim19 – Precipitation of Coldest Quarter      |                                                                                                                         |
|           | bioclim2 – Mean Diurnal Range                     |                                                                                                                         |
|           | bioclim3 – Isothermality                          |                                                                                                                         |
|           | bioclim4 – Temperature Seasonality                |                                                                                                                         |
|           | bioclim5 – Max Temperature of Warmest Month       |                                                                                                                         |
|           | bioclim6 – Min Temperature of Coldest Month       |                                                                                                                         |
|           | bioclim7 – Temperature Annual Range               |                                                                                                                         |
|           | bioclim8 – Mean Temperature of Wettest Quarter    |                                                                                                                         |
|           | bioclim9 – Mean Temperature of Driest Quarter     |                                                                                                                         |
| 83        | tavg_annual                                      | This column indicates Annual Average Temperature.                                                                        |
| 84        | windannual                                       | This column indicates average wind speed annually.                                                                       |
| 85        | solarannual                                      | This column indicates solar radiation annually for each respective region.                                              |
| 86        | precannual                                       | This column indicates precipitation annually for each region.                                                            |
| 87        | vaporannual                                      | This column indicates the average water vapor pressure for each respective region.                                      |
# databda
