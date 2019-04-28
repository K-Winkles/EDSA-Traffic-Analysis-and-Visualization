## EDSA-Traffic-Analysis-and-Visualization

This mini-project is an exercise in the use of Python and some of its tools.

#### Data Extraction
  * Beautiful Soup
  * Scrapy
#### Analysis
  * Numpy
  * Pandas
  * Scikit-learn
#### Visualization
  * Matplotlib

MMDA provides traffic data for all major lines in Metro Manila. For this mini-project, EDSA traffic data will be extracted, analyzed, and visualized from the following link: http://mmdatraffic.interaksyon.com/line-view-edsa.php. Since the data on-site updates periodically, this script is meant to collect the data within a certain timeframe. When the extracted data is deemed sufficient, the visualization of individual roads can then be executed. At this point, all the necessary data has been aquired. Then, analysis will be conducted based on the collected data.

Ideally, the mathematical models that will be applied during data analysis will process the data in a way that it "tells a story". These methods are applicable in numerous contexts that are useful both in theory and in practice as it offers an avenue to accurately predict future conditions. 

### Analysis using Polynomial Regression
At present, the script features polynomial regression as its primary tool of analysis. It is still being tested for reliability and accuracy and is subject to change in the case that it does not perform as well as expected. Alternatively, the script can include all kinds of analysis models and produce both a working model with satisfactory accuracy and a comparison across all models.

#### Additional Non-Core Changes to Follow: 
1. Line name fix
2. Import global libraries since other local imports are redundant
