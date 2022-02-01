# Programming1FinalAssignment

People in poverty may be forced to buy lesser food, a lesser house and have less money to spend on hobbies. Due to these reasons cancer may occur more often among people living in poverty than among people living above the poverty line. In order to find an answer to this several datasets were used. Two datasets containing the municipalities in 2010 and 2018 were used. These were required because the data containing the information about cancer incidents only contained the information per province, rather than municipality. Therefore one final dataset was required as well. This datafile contained information about which municipality is located in which province. Combining all of these datasets made it possible to make a table containing the poverty and social assistance probabilities with the number of cancer incidents per province. Using this dataframe several visualisations were created to find an answer to the research question.

# Research Question
## Does cancer occur more often in provinces which have a high poverty probability?

# Hypothesis
## Cancer occurs more often in provinces with a high poverty probability.


# Required Files

1. [Municipalities 2010](https://www.cbs.nl/nl-nl/onze-diensten/methoden/classificaties/overig/gemeentelijke-indelingen-per-jaar/gemeentelijke-indelingen-alfabetisch-en-numeriek/gemeenten-alfabetisch-per-provincie-2015/gemeenten-alfabetisch-per-provincie-2010)
2. [Municipalities 2018](https://www.cbs.nl/nl-nl/cijfers/detail/83859NED)
3. [Cancer Incidents](https://iknl.nl/nkr-cijfers?fs%7Cepidemiologie_id=506&fs%7Ctumor_id=1&fs%7Cregio_id=525%2C527%2C529%2C521%2C528%2C526%2C520%2C522%2C518%2C519%2C523%2C524&fs%7Cperiode_id=568%2C570%2C572%2C545&fs%7Cgeslacht_id=623&fs%7Cleeftijdsgroep_id=656&fs%7Cjaren_na_diagnose_id=666&fs%7Ceenheid_id=683&cs%7Ctype=line&cs%7CxAxis=periode_id&cs%7Cseries=regio_id&ts%7CrowDimensions=periode_id&ts%7CcolumnDimensions=regio_id&lang%7Clanguage=nl)
4. [Municipalities per Province](https://digitaal.scp.nl/armoedeinkaart2019/waar-wonen-de-armen-in-nederland/)

# Visualisations
## Bubbleplot
Several visualisations are produced to try and find an answer to the research question and prove/disprove the hypothesis. 
The first visualisation is a bubble plot. The x-axis of this plot contains the poverty probability, the y-axis contains the social assistance probability and the size of the bubbles describes the number of cancer incidents. Each bubble contains the information of a province for a selected year. The year can be changed via the slider located above the bubble plot. The information of specific provinces can be turned off by selecting that province from the legend.

## Boxplot
In addition to the bubbleplot, a boxplot has been created as well. The boxplots show the spread of data of a specific type(either poverty probability, social assistance probability or number of cancer incidents) for the years 2011, 2013, 2015 and 2017 in the provinces of the Netherlands. Note that the boxplots are created per year, not per province. The variable for which to see the spread of the data can be selected via the dropdown menu located above the plot.

## Heatmap
The final visualisation that created is a heatmap. Before constructing the heatmap the poverty probability and number of cancer incidents were changed to be categorial data. This was achieved by determining the 1st and 3rd quatiles of both data arrays. If a value was lower than the 1st quantile it would be considered low, if it was higher than the third quantile it would be considered high. If the value was in between the 3rd and 1st quantile it would be considered medium. From this a contingency table could be constructed. The contigency table is then used to draw the heatmap. The heatmap shows the number of combination of poverty and cancer levels.

In addition to the visualisation correlations tables were constructed as well. This was to research the relation between poverty and cancer incidents. The bubble plot provided this information as well, but it is worthwile to connect a number to this. Two kinds of correlation plots are created, one using the standard pearson method and one using the spearman method. spearman was used because the data is non-linear. Therefore, pearson may not provide any significant information.
