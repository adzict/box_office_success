# Box Office Success Determinants

As part of my mentorship, I was tasked to imagine being a Data Scientist for a Top Movie Studio. After a series of box office flops, the producers of the said studio are starting to question their strategy and need some direction. I suggest a new approach - using data to determine what factors go into making a successful film. Luckily, I have a dataset of over 5000 films to mine for insights. My producers ask me to spend some time analyzing the data and present a report detailing your findings, along with recommendations on how to revamp the studio’s strategy.

In order to analyze data and find best recommendations for the studio, I formed a couple of questions I found to be worth answering as the studio can with use that information with certainty to implement changes. The questions asked were:

* What is the correlation between budget and profit? Which budget ranges should be considered for making a Box Office success?
* Do actors/actresses and directors play a role in a movie's success?
* How does a movie's score rating impact profit?
* How does the trend of profit, revenue, profit margin, and other attributes change over years, and can it be relevant to future strategy?
* How do genres play in with profit and profit margin?
* Is there a pattern in common plot keywords with successful movies?
* Are duration and content rating relevant to profit?
* What can we learn from number of votes, and critic reviews in regards to genres and profit?

## Dataset

You can find dataset I used for this project on Kaggle: [movies.csv] (https://www.kaggle.com/carolzhangdc/imdb-5000-movie-dataset) or download it from the repository.


## Most important findings

* What is the correlation between budget and profit? Which budget ranges should be considered for making a Box Office success?
  * Strategy recommendation: The optimal budget value for making a successfull movie should not be less than $40 MM, and on average we recommend it to be somewhere around $75 MM, as on average these budgets result with a good profit margin above 0.6.(This recommendation was made based on a profit margin greater than 0.6.) There is evidence that higher budget movies risk a smaller profit margin, as shown in the aforementioned plot, therefore we cannot recommend very large budgets to be a certain indicator of a Box Office success.

* Do actors/actresses and directors play a role in a movie's success?
  * Strategy recommendation: With great certainty we can recommend that the studio takes into account the VAR score of an actor or an actress, and even more the VAR score of the person who will direct the movie:
    - For actors and actresses we recommend a minimum VAR value to be 1.0, and preferably 3.0 on average.
    - For directors we recommend a VAR value not less than 1.0, and on average 2.53.

* How does a movie's score rating impact profit?
  * Strategy recommendation: We recommend taking into account the average movie score (not less than 7.0) of a director, when hiring one. We consider it will have a positive impact on profit. Another recommendation regarding movie scores will be in relation to movie's genre, and will be detailed later in the report.

* How do genres play in with profit and profit margin?
  * Strategy recommendation: We recommend investing in the Animation genre, in the above mentioned budget ranger of $40MM to $75MM, as well as Family and Adventure genres, as they show a desirable ROI, and are not as expensive. They can be on the lower end of the budget recommendations.

* Are duration and content rating relevant to profit?
  * Strategy recommendation: Focus on PG-13 movies, as the most common profitable genres (Animation, Adventure, Family) are in this group.

## Conclusion and Future recommendations

We recommend including data on oscar winning directors, actors / actresses, and movies, as well as demographic information of users, and movie studios, in the dataset in order to obtain more detailed analysis.

## Acknowledgements

Thanks to [jeremy-lee93](https://github.com/jeremy-lee93/dsc-mod-1-project-v2-1-onl01-dtsc-pt-052620) for an inspiration regarding the VAR values, as well as exploring the profit margin, genres, and the general structure. 

## Contact

Find me on [LinkedIn] (https://www.linkedin.com/in/tanja-ad%C5%BEi%C4%87/), [Twitter] (https://twitter.com/adzic_tanja) or [adzictanja.com] (https://adzict.github.io/).

For a detailed analysis of the dataset please refer to my Medium Blog Post: [Box Office Success Determinants](https://adzic-tanja.medium.com/box-office-success-determinants-c1450fea99ea)
