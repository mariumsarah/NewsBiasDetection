[![OpenSources Data](https://img.shields.io/badge/Data-OpenSources-blue.svg)](https://deepblue.lib.umich.edu/data/concern/data_sets/8w32r569d?locale=en)

# News Bias Detection

This is an open source dataset composed of news articles from Breitbart and DailyKos scraped from a list of articles that were provided by [Deep Blue Data, University of Michigan](https://deepblue.lib.umich.edu/data/concern/data_sets/8w32r569d?locale=en) with the appropriate link and the bias levels on a scale of 1 to 5 for each article towards Democrat and Republican Political Parties. This dataset is intended for use in traning deep learning algorithms.

## How was the dataset created?

This dataset was created by scraping (using the BeautifulSoup package) the articles from links provided on Deep Blue Data, then we modified the extracted CSV file to calculate the BiasTowards Binary Classification as Democrat or Republican based on the scale from 1 to 5 or Negataive to Positive that was intially tagged based on the answers to questions given to the workers about the bias towards Democrat and Republican. For example: One article is tagged as Republican: SomewhatPostive, Democrat: NegativeThis means the article is favouring the Republican Party.

## Formatting

The articles.csv file consists of the intial dataset that was extracted from [Deep Blue Data, University of Michigan](https://deepblue.lib.umich.edu/data/concern/data_sets/8w32r569d?locale=en) and modified to include the BiasTowards Binary Value = Democrat and Republican

Articlesheadlinescontent-updated.csv consists of all articles from Breitbart and DailyKos with their headline and content web-scraped from each HTML Web Page provided.

## Scraping

ArticlesExtracted.ipynb consists of the code that is used to scrape the articles from the two News outlets. 

## Limitations

The dataset does not include all the articles from all the outlets provided in the Open-Source Deep Blue Data that was used. 

## Acknowledgments
- [https://deepblue.lib.umich.edu/data/concern/data_sets/8w32r569d?locale=en](https://deepblue.lib.umich.edu/data/concern/data_sets/8w32r569d?locale=en)
- [https://www.dailykos.com/](https://www.dailykos.com/)
- [https://www.breitbart.com/](https://www.breitbart.com/)
