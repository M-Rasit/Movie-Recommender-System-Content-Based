# Hi,

:loudspeaker: In this repository I created a content-based movie recommender system by using TMDB 5000 Movie Dataset from [Kaggle](https://www.kaggle.com/tmdb/tmdb-movie-metadata).

:loudspeaker: There are 4803 movie in this dataset and we have 20 features. A few columns have dictionary like string data and I used literal_eval function from ast library for extracting values.

:film_projector: Top three rows in the dataset:

![Dataset](https://github.com/M-Rasit/Movie-Recommender-System-Content-Based/blob/master/image/df.head(3).png)

:film_projector: After extracting values from dictionaries, I created a frequency dictionary for genres.

![Genres](https://github.com/M-Rasit/Movie-Recommender-System-Content-Based/blob/master/image/genre.png)

:loudspeaker: I used four methods in this notebook. First, I applied Tf-IdfVectorizer on genre, keywords and overview columns seperately.
Then, I combined transformed (Tf-Idf applied) form of three features. At last, I used linear_kernel for acquiring similarity matrix which will displays similarity of each movies. 
I chose Star Wars and Fury for further process.

:film_projector: Genre - Star Wars

![](https://github.com/M-Rasit/Movie-Recommender-System-Content-Based/blob/master/image/Star%20Wars%20Genre.png?raw=true)

:film_projector: Genre - Fury

![](https://github.com/M-Rasit/Movie-Recommender-System-Content-Based/blob/master/image/Fury%20-%20Genre.png?raw=true)

:film_projector: Keywords - Star Wars

![](https://github.com/M-Rasit/Movie-Recommender-System-Content-Based/blob/master/image/Star%20Wars%20-%20Keywords.png?raw=true)

:film_projector: Keywords - Fury

![](https://github.com/M-Rasit/Movie-Recommender-System-Content-Based/blob/master/image/Fury%20-%20Keywords.png?raw=true)

:film_projector: Overview - Star Wars

![](https://github.com/M-Rasit/Movie-Recommender-System-Content-Based/blob/master/image/Star%20Wars%20-%20Overview.png?raw=true)

:film_projector: Overview - Fury

![](https://github.com/M-Rasit/Movie-Recommender-System-Content-Based/blob/master/image/Fury%20-%20Overview.png?raw=true)

:film_projector: Combined - Star Wars

![](https://github.com/M-Rasit/Movie-Recommender-System-Content-Based/blob/master/image/Star%20Wars%20-%20Combine.png?raw=true)

:film_projector: Combined - Fury

![](https://github.com/M-Rasit/Movie-Recommender-System-Content-Based/blob/master/image/Fury%20-%20Combine.png?raw=true)

### Conclusion

:bangbang: Tf-IdfVectorizer is very effective method and it can be easily concluded that large corpus returns more accurate results. Genre column is important but vectorizer finds more similarities due to lack of differences. For this dataset, combining three features while holding the characteristics of their seperate matrix gets more accurate solution and best recommendation.

Thank you.
