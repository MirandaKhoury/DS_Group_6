This is the repository for the first project of UVA DS 4002 project group 6: Miranda Khoury, Georgia Davidson, and Brian Bippert. This project involves conducting sentiment analysis on Rick and Morty dialogue to answer the research question: does the average sentiment in each season of Rick and Morty become more negative over time/ni later seasons?

## Section 1: Software and platform

Software used: We used the coding language R and IDE software RStudio to perform sentiment analysis on our scripts dataframe using the Bing, Afinn, and NRC dataframes, as well as to run a one-way ANOVA test to compare the mean sentiment in each season.  

Add-on packages installed with software:
- library(readr)
- library(tidyverse)
- library(tm)
- library(wordcloud)
- library(wordcloud2)
- library(tidytext)
- library(textdata)
- library(reshape2)
- library(RWeka)
- library(knitr)
- library(gridExtra)
- library(grid)
- library(magick)
- library(igraph)
- library(ggraph)
- library(ggsci)
- library(circlize)
- library(radarchart)

Platform: We used the platform Windows for our project. 



## Section 2: Map of documentation
 
Data folder:
- Affin.xls
- Bing.xls
- NRC.xls
- RickAndMortyScripts.xls

Output folder:
- Season1afinn.jpg
- Season2afinn.jpg
- Season3afinn.jpg
- episode_averages.csv
- exploratory_analysis_most_talkative_character.png
- linesperseason.jpg
- average_sentiment_by_season.png
- exploratory_analysis_most_used_nonneutral_words.png
- exploratory_analysis_most_used_words.png
- one_way_anova_results_summary.png


Scripts folder:
- rickandmorty.Rmd



## Section 3: Instructions for reproducing results

To replicate our results, first download all four of the .xls files in the Data folder. If not already installed, install R and RStudio. You can download R by selecting one of the mirrors from this site (https://cran.r-project.org/mirrors.html) and selecting “Download R for [your operating system]”. You can download RStudio from this site (https://posit.co/download/rstudio-desktop/).

Download the master script file from the Scripts folder entitled rickandmorty.Rmd and ensure that the master script file is in the working directory of RStudio. To do this, either move the file into the current working directory or set the working directory to the location where the file is stored. Getwd() will return the current working directory and setwd() will change the working directory. Open the rickandmorty.Rmd file. Change the paths in the Import Data cell on lines 46 to 51 to point to the locations of the four data files. Run all cells of the R Markdown script. The script will automatically read in the data files, clean them, perform exploratory analysis, and perform sentiment analysis and related hypothesis testing. Cross reference the outputs provided against the outputs uploaded in the Outputs folder to verify the results.
