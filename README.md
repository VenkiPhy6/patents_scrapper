# Patents Scraper project
Author: Venkatesh Subramanian
Date: June 28, 2024

Welcome! If you need a quick look at the final product of this project, click on the `02_data_viz.ipynb` file in this repository.

## Purpose

- General purpose: Design a dynamic web scraper of patents from the search results of `patents.google.com` and visualize the resulting patents data
- Specific objective: Visualize the data on patents that specify the phrase "international depository authority" within their text
	- For more context on my research here: International Depository Authority are labs around the world that can store samples of microorganisms for patenting purposes. These institutions were created by countries that are members of the World Intellectual Property Organization (WIPO) under the terms of the [Budapest Treaty on Deposit of Microorganisms](https://www.wipo.int/treaties/en/registration/budapest)

Note that although the USPTO provides the [PatentsView API](https://search.patentsview.org/docs/), it can't be used for my specific objective. This API contains full text only for patents post-2023. In addition, it only US patents while I need patents citing international depository authorities across the world!

## The final product

The final product is the visualizations found in `02_data_viz.ipynb`. You can 

## Reading the codebase

As of June 28, 2024, the codebase has 3 notebooks:

1. `00_google_pats_scraping.ipynb` - Contains code for dynamic scraping of top 1000 patents in a search result page of `patents.google.com`
2. `01_data_making.ipynb` - Contains code for cleaning up scraped patent pages from `patents.google.com` and getting specific attributes
3. `02_data_viz.ipynb` - Contains code for visualizing patent utility and ownership

## Running the code

To run the code here locally, follow the steps below.

1. Clone this repository into your local folder.
2. Open a terminal window, create a virutal environment and activate it.
    - Steps for creating and activating virtual environments in different operating systems can be found [in the Python docs](https://docs.python.org/3/library/venv.html).
    - Alternatively, one can use conda environments or simply use the global environment (although I won't advise the latter!).
3. Now in the same terminal window of step 2, `cd` to local folder containing the repository.
	- If you cloned the reposioty into "D:\my_projects\patents_scraper" you would do `cd "D:\my_projects\patents_scraper"`
4. Run `pip install -r requirements.txt`
    - If there are errors in install certain packages, it is upto you to fix them!
5. Once step 4 is successful, you can open the 3 notebooks of the codebase (mentioned in the previous section) and run the cells as you wish.