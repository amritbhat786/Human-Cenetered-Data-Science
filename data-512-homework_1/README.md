# Professionalism & Reproducibility

**DATA 512: Human-Centered Data Science**

**Homework 1**

[![MIT License](https://img.shields.io/apm/l/atomic-design-ui.svg?)](https://github.com/amritbhat786/Human-Cenetered-Data-Science/blob/main/LICENSE)

The goal of this assignment is to construct, analyze, and publish a dataset of monthly article traffic for a select set of pages from English Wikipedia from January 1, 2015 through September 30, 2022.

### Library installation required
 - pandas
 - tqdm
 - seaborn


Data Source: [Wikipedia REST API Endpoint](https://wikimedia.org/api/rest_v1/#/Pageviews%20data/get_metrics_pageviews_per_article__project___access___agent___article___granularity___start___end_), licensed under the [CC-BY-SA 3.0]( CC-BY-SA 3.0 and GFDL licenses) and [GFDL licenses]( CC-BY-SA 3.0 and GFDL licenses).

Data Documentation: [Pageviews API Documentation](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews)

Data Terms of Use: [Wikimedia Foundation REST API terms of use](https://www.mediawiki.org/wiki/REST_API#Terms_and_conditions)

### Input Data Files
List of Dinosaur Articles: data/dinosaur_genera.cleaned.SEPT.2022.csv

### Output Files

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
