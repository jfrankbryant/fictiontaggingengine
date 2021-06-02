<p><b>Motivation </b><br>
This is a repository for my Udacity Data Scientist Nanodegree Introduction to Data Science: Capstone Project: Tagging Engines. <br>
 <br>
I created this dataset to build an algorithm to tag pieces of fiction.</p>

<b>Necessary Libraries:</b> <br>
Pandas  <br>
NumPy <br>
BeautifulSoup <br>
Time <br>
OS <br>
SQLAlchemy <br>
SQLite3 <br>
WordCloud <br>
Matplotlib <br>
Seaborn <br>
Pickle <br>
NLTK <br>
Scikit-Learn <br>

<b>Files in the Repository w/ Summary</b> <br>
AO3_EDA.ipynb: jupyter notebook with exploratory data analysis of the AO3 fanfic dataset <br>
AO3_ETLPipeline.ipynb: jupyter notebook with ETL pipeline for AO3 fanfics <br>
AO3_MLPipeline.ipynb: jupyter notebook with ML pipeline for AO3 fanfics <br>
Fanfic_HTML folder: AO3 fanfics downloaded in HTML format <br>
fictionTaggingEngine.db: SQLite database with processed dataset stored in tables <br>
inProcessAO3data.csv: CSV file with dataset prior to manual tag processing <br>
README.md: documentation file <br>
tags_CSV folder: <br>
  allTags.csv: CSV file with from additionalTags column grouped <br>
  FandomGenreCWTagClustering.xlsx: Excel file with tags with grouped tags, fandoms, and fandom genres in separate sheets <br>
  fandomGenreTags.csv: CSV file with tags of the genres for the fandoms column grouped <br>
  fandomTags.csv: CSV file with tags from fandoms column grouped <br>
UniqueList_fandom.csv: CSV file with a list of fandoms <br>
UniqueList_additionalTags.csv: CSV file with a list of tags from additionalTags column <br>
UniqueList_category.csv: CSV file with a list of tags from category column <br>
UniqueList_character.csv: CSV file with a list of tags from character column <br>
UniqueList_relationships.csv: CSV file with a list of tags from relationships column <br>
fandomGenreCloud.png: word cloud image with fandom genre tags <br>
tagCloud.png: word cloud image with theme tags <br>
illnessTags.png: bar graph with illness tags <br>
characterOfColorTags.png: bar graph with character of color tags <br>
lgbtqiaUmbrellaTags.png: bar graph with LGBTQIA umbrella tags <br>
disabilityTags.png: bar graph with disability tags <br>
fictionTaggingEngine.pkl: saved model of the fiction tagging engine <br>
MLPipelineClassificationReports.xlsx: Excel spreadsheet with classification reports from the different grid search best estimator models <br>

<p><b>Summary of Project Results</b>: <br>
I setup an ETL pipeline to transform AO3 fanfic into a labelled dataset because AO3 has an award-winning tag wrangling system, so out of all of the options it was the best one to get labelled data with the least amount of manual processing. I also setup a machine learning pipeline to create an initial algorithm based on the toy dataset I created. Currently precision is better in the algorithm than recall, however higher recall and f-scores likely need more data with better labelling to train on.</p>

<b>Sources for code adapted and used</b>:  <br>
Stripping code found here: https://stackoverflow.com/questions/7984169/remove-trailing-newline-from-the-elements-of-a-string-list  <br>
Merge fanfics back in a single row: https://stackoverflow.com/questions/39646345/pandas-merging-rows-with-the-same-value-and-same-index <br>
Convert list to string: https://www.geeksforgeeks.org/python-program-to-convert-a-list-to-string/ <br>
Flattened list of lists: https://stackoverflow.com/questions/952914/how-to-make-a-flat-list-out-of-list-of-lists <br>
Word cloud code: <br>
                https://www.geeksforgeeks.org/generating-word-cloud-python/ <br>
                https://www.datacamp.com/community/tutorials/wordcloud-python <br>
                https://towardsdatascience.com/simple-wordcloud-in-python-2ae54a9f58e5 <br>
Code for the ML/NLP pipeline adapted from my Disaster Response Pipelines code: https://github.com/jfrankbryant/dsnd_disasterresponsepipeline <br>
Code for the customized scorers adapted from here: https://stackoverflow.com/questions/52539986/scoring-in-gridsearch-cv?rq=1 <br>
