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
Fanfic_HTML folder: AO3 fanfics downloaded in HTML format
fictionTaggingEngine.db: SQLite database with processed dataset stored in tables
inProcessAO3data.csv: dataset prior to manual tag processing
README.md: documentation file
tags_CSV folder:
  allTags.csv: CSV file with from additionalTags column grouped
  FandomGenreCWTagClustering.xlsx: Excel file with tags with grouped tags, fandoms, and fandom genres in separate sheets
  fandomGenreTags.csv: CSV file with tags of the genres for the fandoms column grouped
  fandomTags.csv: CSV file with tags from fandoms column grouped
UniqueList_fandom.csv: CSV file with a list of fandoms
UniqueList_additionalTags.csv: CSV file with a list of tags from additionalTags column


Sources for code adapted and used:
Stripping code found here: https://stackoverflow.com/questions/7984169/remove-trailing-newline-from-the-elements-of-a-string-list
Merge fanfics back in a single row: https://stackoverflow.com/questions/39646345/pandas-merging-rows-with-the-same-value-and-same-index
Convert list to string: https://www.geeksforgeeks.org/python-program-to-convert-a-list-to-string/
Flattened list of lists: https://stackoverflow.com/questions/952914/how-to-make-a-flat-list-out-of-list-of-lists
