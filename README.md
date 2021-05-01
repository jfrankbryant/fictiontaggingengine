Motivation
This is a repository for my Udacity Data Scientist Nanodegree Introduction to Data Science: Capstone Project: Tagging Engines.

I created this dataset to build an algorithm to tag pieces of fiction.

Necessary Libraries
Pandas
NumPy
BeautifulSoup
Time
OS
SQLAlchemy

Files in the Repository w/ Summary
AO3_ETLPipeline.ipynb: ETL pipeline for AO3 fanfics
Fanfic_HTML folder: 1000 AO3 fanfics downloaded in HTML format
fictionTaggingEngine.db: SQLite database with processed dataset stored in tables
inProcessAO3data.csv: dataset prior to manual tag processing
README.md: documentation file
tags_CSV folder:
  contentWarningTags.csv: CSV file with contentWarning-esque tags from additionalTags column grouped
  FandomGenreCWTagClustering.xlsx: Excel file with tags with grouped tags, fandoms, and fandom genres in separate sheets
  fandomGenreTags.csv: CSV file with tags of the genres for the fandoms column grouped
  fandomTags.csv: CSV file with tags from fandoms column grouped
  themeTags.csv: CSV file with the theme tags from additionalTags column grouped
UniqueFandomList.csv: list of fandoms
UniqueTagList.csv: list of tags from additionalTags column
