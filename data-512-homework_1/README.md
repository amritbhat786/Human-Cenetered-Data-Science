# Considering Bias in Data

**DATA 512: Human-Centered Data Science**

**Homework 1**

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

Data Documentation: [Pageviews API Documentation](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews)

Data Terms of Use: [Wikimedia Foundation REST API terms of use](https://www.mediawiki.org/wiki/REST_API#Terms_and_conditions)

### Library installation required
 - pandas
 - tqdm
 - seaborn


### Input Data Files
List of Dinosaur Articles: data/dinosaur_genera.cleaned.SEPT.2022.csv

### Output Files

```bash
└── data-512-homework_1
    ├── README.md
    ├── data
    │   ├── dino_monthly_cumulative_201507-202209.json
    │   ├── dino_monthly_desktop_201507-202209.json
    │   ├── dino_monthly_mobile_201507-202209.json
    │   ├── dinosaur_genera.cleaned.SEPT.2022.csv
    │   └── pageview_download.json
    ├── results
    │   ├── Fewest_months_plot.png
    │   ├── Max_Min_Average_plot.png
    │   └── Top_10_Peak_Page_Views_plot.png
    └── src
        ├── data_prep.ipynb
        └── dino_analysis.ipynb
```

**JSON Files**
- data/dino_monthly_cumulative_201507-202209.json
- data/dino_monthly_mobile_201507-202209.json
- data/dino_monthly_desktop_201507-202209.json

**Plots (.png files)**

- Plots/Maximum Average and Minimum Average.png
![Maximum Average and Minimum Average.](https://github.com/amritbhat786/Human-Cenetered-Data-Science/blob/main/data-512-homework_1/results/Max_Min_Average_plot.png)

- Plots/Top 10 Peak Page Views.png
![Top 10 Peak Page Views](https://github.com/amritbhat786/Human-Cenetered-Data-Science/blob/main/data-512-homework_1/results/Top_10_Peak_Page_Views_plot.png)

- Plots/Fewest Months of Data.png
![Fewest Months of Data](https://github.com/amritbhat786/Human-Cenetered-Data-Science/blob/main/data-512-homework_1/results/Fewest_months_plot.png)
