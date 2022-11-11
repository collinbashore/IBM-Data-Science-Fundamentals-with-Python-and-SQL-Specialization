# Course #5: Python Project for Data Science

<p align = "center">
<img src = "python-project-for-data-science.png">
</p>

## Project: Extracting and Visualizing Stock Data
**Objective:** You will assume the role of a Data Scientist / Data Analyst working for a new startup investment firm that helps customers invest their money in stocks. Your job is to extract financial data like historical share price and quarterly revenue reportings from various sources using Python libraries and webscraping on popular stocks. After collecting this data you will visualize it in a dashboard to identify patterns or trends. The stocks we will work with are Tesla and GameStop.

- The notebook foile for this project can be found here.

### Python Libraries used/imported:
```import yfinance as yf
import yfinance as yf
import pandas as pd
import requests
from bs4 import BeautifulSoup
import plotly.graph_objects as go
from plotly.subplots import make_subplots
```

### Webscraping
The following webpages were scraped in this project

- For Tesla Stock: [https://www.macrotrends.net/stocks/charts/TSLA/tesla/revenue](https://www.macrotrends.net/stocks/charts/TSLA/tesla/revenue)

- For GameStop Stock: [https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0220EN-SkillsNetwork/labs/project/stock.html](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0220EN-SkillsNetwork/labs/project/stock.html)
  
### Dashboards Produced
These stock dashboards were produced using the [Python Plotly library](https://plotly.com/python/). The dashboards can also be accessed in the notebook file here.

**NOTE:** The data used to produce these dashboards only records the data up to June 2021.

#### Tesla (TSLA) Stock Dashboard
<img src = "Tesla Stock Dashboard.png">



#### GameStop (GME) Stock Dashboard
<img src = "GameStop Stock Dashboard.png"> 







