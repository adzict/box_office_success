# Box Office Success Determinants

![box_office_header](https://github.com/adzict/box_office_determinants/blob/main/assets/box%20office%20header.jpg)

## Table of Contents

1. [ Project Introduction ](#Project_Introduction)
2. [ Technologies Used ](#Technologies_Used)    
3. [ Methods Used ](#Methods_Used)
4. [ Project Description ](#Project_Description)
   * [ 1. Data Sources ](#Data_Sources)
   * [ 2. File Descriptions ](#File_Descriptions) 
5. [ Feature Notebooks and Deliverables ](#Notebooks_deliverables)
6. [ Most Important Findings ](#Findings)
   * [1. What is the correlation between budget and profit? Which budget ranges should be considered for making a Box Office success?](#budget_profit)
   * [2. Do actors/actresses and directors play a role in a movie's success?](#var)
   * [3. How does a movie's score rating impact profit?](#score)
   * [4. How do genres play in with profit and profit margin?](#genres)
   * [5. Are duration and content rating relevant to profit?](#duration_rating)
   * [6. Conclusion and Feature Recommendations](#conclusion)
7. [ Acknowledgments ](#Acknowledgments)
8. [ Licences ](#Licences)
9. [ Contact ](#Contact)

## Project Introduction
<a name="Project_Introduction"></a>

The goal of this project was to recommend strategies for a Movie Studio on how to make a Box Office success.

## Technologies Used
<a name="Technologies_Used"></a>
* [Python](https://www.python.org/)
* [Numpy](https://numpy.org/)
* [Pandas](https://pandas.pydata.org/)
* [Matplotlib](https://matplotlib.org/)
* [Seaborn](https://seaborn.pydata.org/)
* [NLTK](https://www.nltk.org/)

## Methods Used
<a name="Methods_Used"></a>
* Data Processing / Data Cleaning
* Data Analysis
* Descriptive Statistics
* Feature Engineering
* Data Visualization
* Reporting

## Project Description
<a name="Project_Description"></a>
As part of my mentorship, I was tasked to imagine being a Data Scientist for a Top Movie Studio. After a series of box office flops, the producers of the said studio are starting to question their strategy and need some direction. I suggest a new approach - using data to determine what factors go into making a successful film. Luckily, I have a dataset of over 5000 films to mine for insights. My producers ask me to spend some time analyzing the data and present a report detailing your findings, along with recommendations on how to revamp the studio’s strategy.

In order to analyze data and find best recommendations for the studio, I explored a couple of questions based on reasearch and various assumptions:

* What is the correlation between budget and profit? Which budget ranges should be considered for making a Box Office success?
* Do actors/actresses and directors play a role in a movie's success?
* How does a movie's score rating impact profit?
* How does the trend of profit, revenue, profit margin, and other attributes change over years, and can it be relevant to future strategy?
* How do genres play in with profit and profit margin?
* Is there a pattern in common plot keywords with successful movies?
* Are duration and content rating relevant to profit?
* What can we learn from number of votes, and critic reviews in regard to genres and profit?

### Data Sources
<a name="Data_Sources"></a>
The dataset for this analysis was downloaded from the Kaggle website: [movie_dataset.csv](https://www.kaggle.com/carolzhangdc/imdb-5000-movie-dataset)

### File Descriptions
<a name="File_Descriptions"></a>
* [Data](https://github.com/adzict/box_office_determinants/tree/main/data) - folder containing raw and processed data
    * movie_data.csv
    * movies_preprocessed.csv
* [Assets](https://github.com/adzict/box_office_determinants/tree/main/assets) - folder containing all images used for Readme.md, presentation, and blog posts.
* [1. Data Preprocessing and Early EDA](https://github.com/adzict/box_office_determinants/blob/main/1.%20Data%20Preprocessing%20and%20Early%20EDA.ipynb) - notebook containing early data exploration and data cleaning
* [2. Feature Engineering and Data Analysis](https://github.com/adzict/box_office_determinants/blob/main/2.%20Feature%20Engineering%20and%20Data%20Analysis.ipynb) - notebook containing feature engineering and strategy recommendations

## Feature Notebooks and Deliverables
<a name="Notebooks_deliverables"></a>
### Blog Posts
* Blog post on Data Processing and Data Cleaning: [how to | Cleaning and preparing a movie dataset](https://adzic-tanja.medium.com/how-to-cleaning-and-preparing-a-movie-dataset-5dce3cab86f8)
* Blog post on Feature Engineering and Data Analysis: [project | What makes a movie a Box Office succes?](https://adzic-tanja.medium.com/project-what-makes-a-movie-a-box-office-succes-d5cc1dc3c5aa)

### Structure of Notebooks
1. Data Preprocessing and Early EDA
       <ul>
     <li>1. Imports</li>
     <li>2. Data</li>
     <li>3. Early EDA and Data Cleaning </li>
       <ul>
         <li>3.1 Missing values</li>
         <li>3.2 Duplicate rows</li>
         <li>3.3 Outliers and noisiness</li>
         <li>3.4 Mismatched data types</li>
         <li>3.5 Structural errors</li>
         <li>3.6 Saving data for the next stage</li>
       </ul>
   </ul>

3. Feature Engineering and Data Analysis
       <ul>
     <li>1. Imports</li>
     <li>2. Data</li>
     <li>3. Feature Engineering </li>
       <ul>
         <li>3.1 Profit</li>
         <li>3.2 ROI</li>
         <li>3.3 Profit margin</li>
         <li>3.4 VAR (Value Above Replacement)</li>
         <li>3.5 Removing irrelevant features</li>
       </ul>
     <li>4. Data Analysis</li>
       <ul>
         <li>4.1 What is the correlation between budget and profit? Which budget ranges should be considered for making a Box Office success?</li>
         <li>4.2 Do actors/actresses and directors play a role in a movie’s success?</li>
         <li>4.3 How does a movie’s score rating impact profit?</li>
         <li>4.4 How does the trend of profit, revenue, profit margin, and other attributes change over years, and can it be relevant to future strategy?</li>
         <li>4.5 How do genres play in with profit and profit margin?</li>
         <li>4.6 Is there a pattern in common plot keywords with successful movies?</li>
         <li>4.7 Are duration and content rating relevant to profit?</li>
         <li>4.8 What can we learn from number of votes, and critic reviews in regards to genres and profit?</li>
       </ul>  
   </ul>

### Presentation
Link to the presentation: [presentation.pdf]()

## Most Important Findings
<a name="Findings"></a>
### 1. What is the correlation between budget and profit? Which budget ranges should be considered for making a Box Office success?
<a name="budget_profit"></a>
*Visualizing relationship between budget and profit

![budget-profit-linear](https://github.com/adzict/box_office_determinants/blob/main/assets/budget%20profit%20linear.png)

  * <strong>Strategy recommendation:</strong> I recommend that the optimal budget value for making a successful movie should not be less than $40 MM, and on average I recommend it to be somewhere around $75 MM, as on average these budgets result with a good profit margin above 0.6.(This recommendation was made based on a profit margin greater than 0.6.) There is evidence that higher budget movies risk a smaller profit margin, as shown in the analysis, therefore I cannot support the claim that large budgets are a certain indicator of a Box Office success.

![top-30-profit](https://github.com/adzict/box_office_determinants/blob/main/assets/profit%20budget%20top%2030%20profitable.png)

### 2. Do actors/actresses and directors play a role in a movie's success?
<a name="var"></a>
  * <strong>Strategy recommendation:</strong> With great certainty, I can recommend that the studio takes into account the VAR score of an actor or an actress when hiring, and even more so the VAR score of the person who will direct the movie:
    * For actors and actresses, I recommend a range value of VAR between 1.0 and 3.0
    * For directors, I recommend a range value of VAR between 1.0 and 2.50

### 3. How does a movie's score rating impact profit?
<a name="score"></a>
  * <strong>Strategy recommendation:</strong> I recommend taking into account the average movie scores (not less than 7.0) of a director, when hiring one. I consider it might have a positive impact on profit. Another recommendation regarding movie scores will be in relation to movie’s genre, and will be detailed later in the report.

### 4. How do genres play in with profit and profit margin?
<a name="genres"></a>
  * <strong>Strategy recommendation:</strong> I recommend investing in the Animation genre, in the above-mentioned budget range of $40MM to $75MM, as well as Family and Adventure genres, as they show a desirable Return Of Investment, and are not as expensive. Those genres can be on the lower end of the budget recommendations — $40MM.

*Visualizing genres

![genres-count](https://github.com/adzict/box_office_determinants/blob/main/assets/genre%20movie%20count.png)

### 5. Are duration and content rating relevant to profit?
<a name="duration_rating"></a>
  * <strong>Strategy recommendation:</strong> The studio should focus on PG-13 movies, as the most common profitable genres (Animation, Adventure, Family) are in this group.


### 6. Conclusion and Feature Recommendations
<a name="conclusion"></a>
#### Conclusion
The Top Movie Studio producers stated a great business question: What are we doing wrong, and what can we do to change our strategy? Fortunately for them, there are many answers to the question, and some of them were presented in this project. I would separate a couple of important recommendations as part of this conclusion.

The data available showed that budget values between $40 MM and $75 MM, for a good profit margin of 0.6. The most profitable genres are Animation, Adventure, and Family — all three are PG-13 content rating. Also, included in the recommendation, is the importance of directors and actors/actresses. Directors with an average movie score above 7 show great potential to bring significant value to a movie, even so if their VAR score is between 1.0 and 2.5. The same goes for actors/actresses — if their VAR score is between 1.0 and 3.0, they will bring value to a movie.

As the quest for a more detailed analysis and answers is always on, I will include a couple of Future recommendations that I deem to be potentially valuable to the studio.

#### Feature recommendations
I recommend including and exploring data on Oscar winning directors, actors/actresses, and movies. During my time working on this project, I wondered if creating sequels is a good opportunity for a successful movie — this is something I would also consider including. Besides that, I would also add demographic information of users if applicable, and other movie studio box office successes in the dataset in order to obtain more detailed analysis. I believe this information would bring additional insight into assessing determinants of a Box Office success.


## Acknowledgments
<a name="Acknowledgments"></a>
Thanks to [jeremy-lee93](https://github.com/jeremy-lee93/dsc-mod-1-project-v2-1-onl01-dtsc-pt-052620) for an inspiration regarding the VAR values, as well as exploring the profit margin.

## Licenses
<a name="Licences"></a>
[Database Contents License (DbCL) v1.0](https://opendatacommons.org/licenses/dbcl/1-0/)

## Contact
<a name="Contact"></a>
Find me on [LinkedIn](https://www.linkedin.com/in/tanja-ad%C5%BEi%C4%87/), [Twitter](https://twitter.com/adzic_tanja) or [adzictanja.com](https://adzict.github.io/).
