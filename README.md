# World Happiness Report: Exploratory Data Analysis 

The World Happiness Report is a publication that contains the rankings of national happiness of different countries, which is known as the Happiness Score or Subjective Well-being.

The Happiness Score is measured as a result of the national average response to the question "Please imagine a ladder, with steps numbered from 0 at the bottom to 10 at the top. The top of the ladder represents the best possible life
for you and the bottom of the ladder represents the worst possible life for you.
On which step of the ladder would you say you personally feel you stand at this
time?”


There are six other metrics that are also measured along with the happiness score: real GDP per capita, social support, healthy life expectancy, freedom to make life choices, generosity, and perceptions of corruption.

## About the Project

This project is two-fold. First, we will be carrying out EDA on the data for different countries. Secondly, we will be specifically performing EDA on Pakistan's data.

### Data Loading

We are using the world happiness report for the years 2006-2022. The data can be found at https://worldhappiness.report/data/. We are also going to use the world happiness report for 2021 and do some of our analysis on that.

#### Variable Definition

The variables in our dataset are the following:
- Life Ladder: this is the Happiness Score for a country. It answers the question "Please imagine a ladder, with steps numbered from 0 at the
bottom to 10 at the top. The top of the ladder represents the best possible life
for you and the bottom of the ladder represents the worst possible life for you.
On which step of the ladder would you say you personally feel you stand at this
time?” The answer is on a scale of 0-10.
- Log GDP per Capita: GDP per Capita shows the country's GDP divided by its total population. We take log of this because it is easier to plot in our analysis.
- Healthy Life Expectancy at Birth: shows the average life expectancy for the country
- Social Support: this is the national average of the binary responses to the question "If you
were in trouble, do you have relatives or friends you can count on to help you
whenever you need them, or not?"
- Freedom to make life choices: this is the national average of responses to the GWP
question “Are you satisfied or dissatisfied with your freedom to choose what
you do with your life?”
- Generosity: this is the residual of regressing national average of response to the GWP
question “Have you donated money to a charity in the past month?” on GDP
per capita
- Perception of Corruption: The measure is the national average of the survey responses to two questions in the GWP: “Is corruption widespread throughout
the government or not” and “Is corruption widespread within businesses or
not?” The overall perception is just the average of the two 0-or-1 responses.

The data looks like this:

![image](https://github.com/zahra-q/world-happiness-index-EDA-pakistan/assets/58932323/9e8d96ff-4ba8-489d-8537-7742e8831f26)


### Data Cleaning

- We remove missing values
- Drop irrelevant columns

### Exploratory Data Analysis

The steps we carry out are:

- Finding correlations between factors like GDP per capita and Happiness Score.
-  Answering several questions like:

1. What are the correlations between the other factors like Generosity and Log GDP per capita, and the Happiness Score? Is there a correlation at all?
2. Which countries were still the happiest when COVID struck in 2020?
3. What has been the distribution of the Ladder Scores by a) Region and b) Sub Region?
4. What were the top 10 and bottom 10 scoring countries?



Our answers include graphs like the following:

![image](https://github.com/zahra-q/world-happiness-index-EDA-pakistan/assets/58932323/82d86ce3-375b-4ef3-a668-d0f12c799abb)


![image](https://github.com/zahra-q/world-happiness-index-EDA-pakistan/assets/58932323/35456b7f-d5dd-4b62-9621-9659100bb613)

## Happiness Report for Pakistan

For this analysis, we carried out the same steps as above (removing/imputing missing values, dropping columns). Some of the questions we answered were:

1. What has been Pakistan's Ladder score over the years? Its GDP per capita? Social Support?
2. How does Pakistan compare to the rest of South Asia with regards to Ladder score? Generosity? Freedom to make life choices?

### Data Visualization

We created bar charts, line graphs, and distribution graphs to help answer our questions. 


