# Scraper de Discours en Français - French Speech Scraper 

# Résumé français (please see below for english)

## Objectif
Le but de discours_scraper.py est de rassembler sous la forme d'un fichier CSV les récents discours et allocutions prononcés par le gouvernement français à partir du lien suivant: [discours](https://www.vie-publique.fr/discours/recherche?search_api_fulltext_discours=&sort_by=field_date_prononciation_discour&field_intervenant_title=&field_intervenant_qualite=&field_date_prononciation_discour_interval%5Bmin%5D=&field_date_prononciation_discour_interval%5Bmax%5D=&form_build_id=form-7rs-y5DWW6gIk2Mh0Bn1wxLrLl_Qc8QkzymXI0aokUU&form_id=views_exposed_form)

Le résultat est extrait sur la base des colonnes suivantes : 
```titre,date,discours```

Vous pouvez décider du nombre de pages à scraper en renseignant les variables de classe ```pages_begin``` et ```pages_end```.

Ce scraper a été réalisé dans le cadre d'une auto-formation à l'analyse de données textuelles.


## Dépendances requises

* Selenium
* ChromeDriverManager pour éviter de gérer les incompabilités entre la version actuelle de Chrome et celle du driver  

## Avertissement

* Je n'ai pas testé sur colab!! Le script marche sous JupyerLab :-)
* Le script est basé, comme tous les scrapers, sur l'architecture d'un site web. Il est possible que cette dernière change, ou que les sélecteurs css soient à updater. Des ajustements peuvent donc être nécessaires pour récolter les données.

# English Summary

## Purpose

The purpose of discours_scraper.py is to gather in the form of a CSV file the recent speeches delivered by the French government from the following link: [speech](https://www.vie-publique.fr/discours)

The result is extracted on the basis of the following columns: 
```titre,date,discours```

You can choose the number of pages to be scraped by filling the class variables ```pages_begin``` and ```pages_end```.

This scraper was made as part of a self-training in the analysis of textual data.


## Required Dependencies

* Selenium
* ChromeDriverManager to avoid managing incompatibilities between the current version of Chrome and the driver version. 

## Warning
* You may complicate your life if you run the notebook with colab. I have only tested it with JupyterLab :-)
* The script is based, like all scrapers, on the architecture of a website. It is possible that this architecture changes, or that the css selectors need to be updated. Adjustments may therefore be necessary to collect the data.


