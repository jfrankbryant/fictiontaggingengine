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
SQLite3
WordCloud
Matplotlib
Seaborn
Pickle
NLTK
Sklearn (sci-kit learn)

Files in the Repository w/ Summary
AO3_EDA.ipynb: jupyter notebook with exploratory data analysis of the AO3 fanfic dataset
AO3_ETLPipeline.ipynb: jupyter notebook with ETL pipeline for AO3 fanfics
AO3_MLPipeline.ipynb: jupyter notebook with ML pipeline for AO3 fanfics
Fanfic_HTML folder: AO3 fanfics downloaded in HTML format
fictionTaggingEngine.db: SQLite database with processed dataset stored in tables
inProcessAO3data.csv: CSV file with dataset prior to manual tag processing
README.md: documentation file
tags_CSV folder:
  allTags.csv: CSV file with from additionalTags column grouped
  FandomGenreCWTagClustering.xlsx: Excel file with tags with grouped tags, fandoms, and fandom genres in separate sheets
  fandomGenreTags.csv: CSV file with tags of the genres for the fandoms column grouped
  fandomTags.csv: CSV file with tags from fandoms column grouped
UniqueList_fandom.csv: CSV file with a list of fandoms
UniqueList_additionalTags.csv: CSV file with a list of tags from additionalTags column
UniqueList_category.csv: CSV file with a list of tags from category column
UniqueList_character.csv: CSV file with a list of tags from character column
UniqueList_relationships.csv: CSV file with a list of tags from relationships column
fandomGenreCloud.png: word cloud image with fandom genre tags
tagCloud.png: word cloud image with theme tags
illnessTags.png: bar graph with illness tags
characterOfColorTags.png: bar graph with character of color tags
lgbtqiaUmbrellaTags.png: bar graph with LGBTQIA umbrella tags
disabilityTags.png: bar graph with disability tags
fictionTaggingEngine.pkl: saved model of the fiction tagging engine
MLPipelineClassificationReports.xlsx: Excel spreadsheet with classification reports from the different grid search best estimator models

Summary of Project Results:
I setup an ETL pipeline to transform AO3 fanfic into a labelled dataset because AO3 has an award-winning tag wrangling system, so out of all of the options it was the best one to get labelled data with the least amount of manual processing. I also setup a machine learning pipeline to create an initial algorithm based on the toy dataset I created. Currently precision is better in the algorithm than recall, however higher recall and f-scores likely need more data with better labelling to train on.

Sources for code adapted and used:
Stripping code found here: https://stackoverflow.com/questions/7984169/remove-trailing-newline-from-the-elements-of-a-string-list
Merge fanfics back in a single row: https://stackoverflow.com/questions/39646345/pandas-merging-rows-with-the-same-value-and-same-index
Convert list to string: https://www.geeksforgeeks.org/python-program-to-convert-a-list-to-string/
Flattened list of lists: https://stackoverflow.com/questions/952914/how-to-make-a-flat-list-out-of-list-of-lists
Word cloud code:
                https://www.geeksforgeeks.org/generating-word-cloud-python/
                https://www.datacamp.com/community/tutorials/wordcloud-python
                https://towardsdatascience.com/simple-wordcloud-in-python-2ae54a9f58e5
Code for the ML/NLP pipeline adapted from my Disaster Response Pipelines code: https://github.com/jfrankbryant/dsnd_disasterresponsepipeline
Code for the customized scorers adapted from here: https://stackoverflow.com/questions/52539986/scoring-in-gridsearch-cv?rq=1
