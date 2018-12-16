# Analysis and Impacts of Fake News

This course project is developed by Can Yilmaz Altinigne, Günes Yurdakul and Bengisu Güresti.

Data Story link: https://heybeliada.github.io

Data Story repository: https://github.com/heybeliada/heybeliada.github.io

ATTENTION: Map and network may not be seen in Jupyter Notebook. They are visible in Data Story. Also you can find them in static/map.html and network.html

Final notebook can be found in Milestone_3.ipynb

# Abstract
Everybody lies at some point of time. However, if the liar is a popular and respected source or figure in society, this may have crucial effects on people. The goal of this project is to analyze the distribution of lies among the political figures and news sources in the U.S. and the effects of these lies on voters and social media. We use Liar dataset collected from PolitiFact.com and prepared by William Yang Wang. We aim to specify the topics which politicians and news sources mostly lie about. Also, we intend to reveal if the lies told by politicians propagate to other news sources. We would like to emphasize the power of the statements made by notable sources in society. Because, we believe that the manipulation of people's decisions through fake news may have drastic effects on society and democracy in a country. As we are all from Turkey, we are the witnesses of how biased media manipulates the people's political views which determine the future of the country.  

# Research questions

1. What are the subjects that the politicians and news sources mostly lie about?
2. What are the most frequent words used in lies?
3. What are the most frequent words used in lies relating to specific subjects ?
4. What is the total number of lies told by each state representers ?
5. Do republicans and democrats tell lies more in the states that they won or they lost ?
6. Visualization of the truth ratios of the statements made by famous politicians.
7. Trump's False Statements during 2016 Elections Campaign
8. Quarrel Network
9. Creating a lie classifier using Logistic Regression, SVM and LSTM models.

# Dataset
We use Liar dataset collected from PolitiFact.com and prepared by William Yang Wang. The dataset is in tsv format, and also for each row, there is an HTML link column including some additional information about the specific statement. We will parse the dataset as well as the webpage to extract other informations such as statement date and place. The dataset contains train, test and validation sets amd has nearly 12k statements. We will combine them for analysis.

## Liar Dataset Structure:

- Id

- Label

- Statement

- Subject

- Speaker’s Job Title

- Job

- State

- The Party Affiliation

- barely true counts

- false counts

- half true counts

- mostly true counts

- pants on fire counts

- Communication Media

- Date

Additionally, we used US Presidental Election results which we have downloaded from the official website of the United States government https://www.usa.gov/election-results in order to utilize from the election results of each state, since our liar dataset also includes US State column for each sample and political view of speaker of each sample.

# Update in Milestone 2
## Data pre-processing:
    - Added new features by parsing web page where the data is collected from. We added 'Date' column.
    - We decided to use US Presidental Election results in order to utilize from the election results of each state, since our liar dataset also includes US State column for each sample and political view of speaker of each sample.
    - For each US State, we observed the change of votes in percentage since the last election. Additionally, we observed if the winning party is changed or not changed.

## Data Analysis:
    - We change some ambiguous questions that we suggested in the previous milestone to the questions that we can answer quantitatively.
    - In Q1, we calculated the top subjects in the lie statements. We considered 'pants on fire' and 'False' labeled samples as lies. Then, we visualized the results in a histogram.
    - In Q2, we visualised the top 20 specific words in false and pants on fire labeled statements. We realized that the most used words are like (I, you, the) words, which are meaningless in our case. Therefore we used NLTK's stopword library and filtered stopwords in statements out. We selected the words by hand since there are connections between some of the words and also some of the words were irrelevant.
    - We decided to answer Q3 in the next milestone.
    - In Q4, we found the count of lies which have been told in each state. We visualized the results in bar chart and a `Folium` map.
    - In Q5, we compare the means of lie counts samples for Republicans' and Democrats' in the states that they win and lose before 2012 election and 2016 election in order to determine if republicans and democrats tell lies more in the states that they won or they lost.
    
# Update in Milestone 3

    - We completed the analysis of Question 3 (What are the most frequent words that used in lies relating to specific subjects ?)
    - We added the plot of number of Trump's false statements from his candidacy decleration to the election date
    - We visualized the authenticity percentage of the statements made by Barack Obama, Hillary Clinton and Donald Trump.
    - We added a quarrel network which shows lie connection between politicians.
    - We created a lie classifier using several classification models and deep learning models.

# Contribution

Can: Creating network and map visualizations, creating the structure of project webpage, answering several research questions.

Günes: Data preparation, creating the lie classifier, conducting the research on effects of false statements on election results.

Bengisu: Data preparation, creating dataframe queries and categorization functions, answering several research questions.

Günes Yurdakul will be our main presenter during poster presentation.

# A list of internal milestones up until project milestone 3

*04.11.2018:* Download the required dataset

*10.11.2018:* Data wrangling and data preprocessing

*14.11.2018:* Exploratory data analysis and revealing statistics

*16.11.2018:* Scraping and analysis of external HTML part of the dataset

*18.11.2018:* Decide on data visualization techniques

*21.11.2018:* Visualizing our results

*23.11.2018:* Setting a structured notebook to present descriptive analysis on the dataset.

*25.11.2018:* Commenting and debugging our code

*01.12.2018:* Creating more complex research question.

*12.12.2018:* Completing missing research questions and newly added questions.

*16.12.2018:* Completing data story 
