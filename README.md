# airbnb-srilanka
Basic Scrapy spider for Airbnb Sri Lanka


Based on [code by Luca Verginer](http://www.verginer.eu/blog/web-scraping-airbnb/)

# Instructions

- Install scrapy and json using pip, preferably on a virtualenv
- Edit the `QUERY` const on `bnbspider.py` for crawling a different location (`'Contry--City'` syntax, query filter parameters can also be used).
- Run `scrapy crawl bnbspider -o  output.csv`

Additional fields can be added by mapping the properties of the json response to their equivalent AirbnbItem properties on `BnbspiderSpider` (the name is redundant, but whatever) `parse_listing_contents` method.
