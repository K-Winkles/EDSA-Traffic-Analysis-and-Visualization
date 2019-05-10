## EDSA-Traffic-Analysis-and-Visualization

This mini-project is an exercise in the use of Python and some of its tools. More than that, the data extracted by the script will most iikely be of use later on.

#### Data Extraction
  * Beautiful Soup
  * Scrapy
  * Selenium 
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

## EDSA Traffic Data: Analysis

After an extraction period of 7 days, sufficient data has been collected in order to start munging. Pre-processing will be executed in the following manner:
1. Collate data from raw .csv files
2. Separate aforementioned data into two 2-dimensional numpy arrays (southbound and northbound)
3. Place data in such a way that it is arranged chronologically with respect to the individual lines
4. Take the average for every 4 entries since this represents 1 hour 
The last step is necessary since visualization and line fitting is unhelpful when considering the entire scope of raw data. Breaking the data into several pieces and analysing each set is more conducive for meaningful story telling. As was explained in the previous notebook, polynomial regression is the tool of choice for this task. 

Note that during the 7-day timeframe of data extraction, there was a holiday in the middle of the week. To be more specific, it fell on a Wednesday. This factor will be taken into consideration when analyzing individual days. 
