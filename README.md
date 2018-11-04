# Analysis and Impacts of Fake News

# Abstract
Everybody lies at some point of time. However, if the liar is a popular and respected source or figure in society, this may have crucial effects on people. The goal of this project is to analyze the distribution of lies among the political figures and news sources in the U.S. and the effects of these lies on voters and social media. We use Liar dataset collected from PolitiFact.com and prepared by William Yang Wang. We aim to specify the topics which politicians and news sources mostly lie about. Also, we intend to reveal if the lies told by politicians propagate to other news sources. We would like to emphasize the power of the statements made by notable sources in society. Because, we believe that the manipulation of people's decisions through fake news may have drastic effects on society and democracy in a country. As we are all from Turkey, we are the witnesses of how biased media manipulates the people's political views which determine the future of the country.  

# Research questions 
- Do republicans or democrats lie more?
- What are the subjects that the politicians and news sources mostly lie about?
- What are the effects of lies told by politicians on news sources?
- What are the effects of lies told by politicians and news sources on votes?
- What are the most frequent words that used in lies?
- Which political side lies more about specific subjects (i.e. abortion, climate change)?

# Dataset
We use Liar dataset collected from PolitiFact.com and prepared by William Yang Wang. The dataset is in tsv format, and also for each row, there is an HTML link column including some additional information about the specific statement. We will parse the dataset as well as the webpage to extract other informations such as statement date and place. The dataset contains train, test and validation sets amd has nearly 12k statements. We will combine them for analysis.

# A list of internal milestones up until project milestone 2

**04.11.2018:** Download the required dataset
**10.11.2018:** Data wrangling and data preprocessing
**14.11.2018:** Exploratory data analysis and revealing statistics
**16.11.2018:** Scraping and analysis of external HTML part of the dataset
**18.11.2018:** Decide on data visualization techniques
**21.11.2018:** Visualizing our results
**23.11.2018:** Setting a structured notebook to present descriptive analysis on the dataset.
**25.11.2018:** Commenting and debugging our code

# Questions for TAa
- Do we present the answers to all research questions in Milestone 2 ?
- Is the dataset we use small, do you suggest to get a bigger dataset ?
