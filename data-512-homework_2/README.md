# Professionalism & Reproducibility

**DATA 512: Human-Centered Data Science**

**Homework 2**

[![MIT License](https://img.shields.io/apm/l/atomic-design-ui.svg?)](https://github.com/amritbhat786/Human-Cenetered-Data-Science/blob/main/LICENSE)

The goal of this assignment is to explore how bias can show up in data using Wikipedia articles. This assignment will consider articles on political figures from different countries.

Data Source:
- [Category:Politicians by nationality](https://en.wikipedia.org/w/index.php?title=Category:Politicians_by_nationality&subcatfrom=South+Sudanese+politicians#mw-subcategories).
- [World Population Data Sheet](https://www.prb.org/international/indicator/population/table)

WikiMedia API:
- Documentation: [API:Info](https://www.mediawiki.org/wiki/API:Info)
- License: [Creative Commons Attribution-ShareAlike License](https://creativecommons.org/licenses/by-sa/3.0/)

ORES API:
- Documentation: [ORES](https://www.mediawiki.org/wiki/ORES)
- License: [Creative Commons Attribution-ShareAlike License](https://creativecommons.org/licenses/by-sa/3.0/)

### Input Data Files
- data/politicians_by_country_SEPT.2022.csv
  - Politicians and their associated country.
- data/population_by_country_2022.csv
  - Countries and their population in millions.

### Output Files
- data/wp_countries-no_match.txt
  - List of all countries for which there are no matches between politician and population data.
- data/wp_politicians_by_country.csv
  - Consolidated data of politician articles, their countries and region, the respective country population and article quality.

### Data Description for wp_politicians_by_country.csv

| Feature         | Data type | Description                                                                    |
|-----------------|-----------|--------------------------------------------------------------------------------|
| country         | String    | The country that the politician belongs to                                     |
| region          | String    | The region that the country belongs to                                         |
| population      | float     | Population of the respective country (in millions, rounded to 1 decimal place) |
| article_title   | String    | The Wikipedia article title of the politician (the politician's name)          |
| revision_id     | float     | The last revision ID of the Wikipedia article                                  |
| article_quality | String    | The quality of the article as predicted by the ORES API                        |


I learnt that the 10 countries with the highest total articles per capita were most those with lower populations and the bottom 10 countries are the ones with some of the highest population. Also that the countries/regions with higher english language usage were the ones with high quality wiki articles, for eg European countries. 

The results have a high chance of being biased as the list of articles scraped from Wikipedia does not contain politician articles from many countries, including major countries like the United States, Canada, Australia, United Kingdom, etc, which was very surprising as these are some of countries with prominent leaders. The exlusion of these data points can cause missing data bias to some extent.


1. What biases did you expect to find in the data (before you started working with it), and why?
- As I started my analysis, I expected there to be a bias based on regions. Regions/ countries with non-english historical literature should have had lower quality articles.

3. What might your results suggest about (English) Wikipedia as a data source?
- As wikipedia is an English language forum, I was expecting high presence of high quality english speaking countries like United States, United Kingdom. However, since these countries are scrapped from the Wikipedia data source, I personally consider it a moderate-highly biased dataset and one not suitable for any correlational analysis nor any pattern mining.

7. How might a researcher supplement or transform this dataset to potentially correct for the limitations/biases you observed?
- A researcher can supplement this dataset by also including information about the percentage of english speaking population in each country. That might present a fair comparison between countries and result in interesting patterns in the data.