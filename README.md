# TAD Pictures Productions Analysis of Movie Studio Profits in the US
This github includes 
- Images 
    - Folder containing the images of our plots
- zippedData
    - folder that contains all the files that we used for our analysis
    - This does not contain im.db 
- [TADProduction.ipynb](/TADProduction.ipynb)
    - Jupyter Notebook containing our analysis
- [Presentation.pdf](/Presentation.pdf)
    - pdf of our powerpoint 
## BLUF 
- Disney has profited the most domestically by over $1B 
- Movies perform best in summer
- The top genres in the US are adventure, comedy and action
## Introduction
TAD Pictures, a theoretical stakeholder, is seeking to create a new movie studio. They are hoping to release movies in the US and maximize profits as they begin this new venture. They have tasked us with analying the movie industry to determine the best practices moving forward.

Data was taken from 3 sources - IMDb, Box Office Mojo, the Numbers. The metric we used for success was domestic profit. Data was taken between the years of 2010 and 2018.
## Table of Contents

- Data Exploring

- Data Cleaning

- Merging the DataFrames

- Visualizations

- Simple Linear Regression Model

- Conclusion

- Sources

- Dashboard

## Data Exploring 
We were given six data files with information on movie performance. Upon exploring the data, we created a master dataset that takes information from the three data files we felt are most relevant to our analysis.
## Data Cleaning
We first normalized the movie titles by removing spaces and punctuation. Then, we renamed each column name in the three datasets to ensure consistency for merging purposes. Additionally, we corrected major movie titles that were spelled differently. Finally, we filtered each dataset to include only entries from 2010 to 2018.
## Merging the DataFrames
We then merged our three datasets into one master dataset. Afterward, we dropped unnecessary columns that weren't needed for our analysis. Next, we calculated our ROI and Profits columns. Finally, we imputed a couple of missing genres and studios for well-known movies. 
## Visualizations
We decided to get the top 25 studios with the highest domestic gross and ROI. 

![Top25StudiosDomesticGross](images/Top25StudiosDomesticGross.png)
![Top25StudiosDomesticROI](images/Top25StudiosDomesticROI.png)

Next we decided to get the top 25 studios and genres with the highest domestic profits.

![Top25StudiosDomesticProfit](images/Top25StudiosDomesticProfit.png)
![Top25GenresDomesticProfit](images/Top25GenresDomesticProfit.png)

Then we got the top 10 profitable movies and the respective studio.

![Top10MoviesDomesticProfit](images/Top10MoviesDomesticProfit.png)

## Simple Linear Regression Model
We then created linear regression model of disney profits over time. Looking at our R-squared value of 0.817 indicates that 81.7% of the model accounts for variation in profit, which we find significant. Therefore we belive Disney experienced a significant change in mean profit over a period of 8 years.
## Conclusion 
Partnering with Disney can be a strategic move for movie producers. The studio's strong brand reputation and extensive market reach can significantly boost a film's profitability. Additionally, working with Disney can lead to increased profits regardless of the release window. While summertime traditionally provides an optimal window for movie releases due to higher audience attendance, collaborating with Disney can elevate profits at any time of the year.

Furthermore, analyzing genre trends reveals that adventure, comedy, and action genres tend to generate the highest profits. By aligning with these popular genres, filmmakers can capitalize on audience preferences and maximize their revenue potential.
## Sources
- [IMDB](https://www.imdb.com/)
- [BoxOfiiceMojo](https://www.boxofficemojo.com/)
- [The Numbers](https://www.the-numbers.com/)
- [Gitnux](https://gitnux.org/entertainment-industry-statistics/#:~:text=Highlights%3A%20The%20Most%20Important%20Entertainment,CAGR%20from%202022%20to%202027)
## Dashboard
- [Tableau](https://public.tableau.com/app/profile/alli.ward/viz/TADMovieStudioAnalysis/Dashboard1?publish=yes)