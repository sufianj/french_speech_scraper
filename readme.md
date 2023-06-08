# Scraper de Discours en Français - French Speech Scraper 


## Purpose

The purpose of discours_scraper.py is to gather in the form of a CSV file the recent speeches delivered by the French government from the following link: [speech](https://www.vie-publique.fr/discours)

The result is extracted on the basis of the following columns: 
```titre,date,discours```

You can choose the number of pages to be scraped by filling the class variables ```pages_begin``` and ```pages_end```. It is quite pratical when your internet connection breaks during the scrapping.

## Update 

08/06/2023: I remark that some of the speeches contains ```<br>``` and not ```<p/>```. Thus I take all the inner html contents and remove the tags afterwards.


## Required Dependencies

* Selenium 4
* ChromeDriverManager to avoid managing incompatibilities between the current version (114, on 8th June 2023) of Chrome and the driver version. 

## Warning
* You may complicate your life if you run the notebook with colab. I have only tested it with JupyterLab :-)
* The script is based, like all scrapers, on the architecture of a website. It is possible that this architecture changes, or that the css selectors need to be updated. Adjustments may therefore be necessary to collect the data.


