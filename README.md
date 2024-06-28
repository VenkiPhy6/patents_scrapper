# Patents Scraper project
Author: Venkatesh Subramanian
Date: June 28, 2024

## Purpose

- General purpose: Design a dynamic web scraper of patents from the search results of `patents.google.com` and visualize the resulting patents data
- Specific objective: Visualize the data on patents that specify the phrase "international depository authority" within their text
	- For more context on my research here: International Depository Authority are labs around the world that can store samples of microorganisms for patenting purposes. These institutions were created by countries that are members of the World Intellectual Property Organization (WIPO) under the terms of the [Budapest Treaty on Deposit of Microorganisms](https://www.wipo.int/treaties/en/registration/budapest)

## Using the codebase

As of June 28, 2024, the codebase has 3 notebooks:

1. `00_google_pats_scraping.ipynb` - Contains code for dynamic scraping of top 1000 patents in a search result page of `patents.google.com`
2. `01_data_making.ipynb` - Contains code for cleaning up scraped patent pages from `patents.google.com` and getting specific attributes
3. `02_data_viz.ipynb` - Contains code for visualizing patent utility and ownership

## The final product

The final product is the visualizations found in `02_data_viz.ipynb`