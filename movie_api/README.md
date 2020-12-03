# File Description:- 
## recommendation.py
Here, we have our logic written for the recommendation algorithm. Consists a total of 5 functions

### get_data():-
- get_data() is used to fetch the data about the movies and return the dataset with it's attributes as the result for further preprocessing.

![alt text](https://miro.medium.com/max/1400/1*XbCH8vioupYE4MjaePyO3w.png)

### combine_data():-
- combine_data() drops the columns not required for feature extraction and then combines the cast and genres column,finally returning the combine column as the result of this function.

![alt text](https://miro.medium.com/max/1400/1*Bjn1UpDksEQpHTWHJ22DTg.png)


### transform_data():-
- transform_data() takes the value returned by combine_data() and the plot column from get_data() and applies CountVectorizer and TfidfVectorizer respectively and calculates the Cosine values.

![alt text](https://miro.medium.com/max/1254/1*DMV5_eytR3aVm7Op7L9PFA.png)

### recommend_movies():-
- recommend_movies() takes four parameters i.e movie_name and return values of get_data(), combine_data(), transform_data as input and returns the top 20 movies similar to our input movie.

![alt text](https://miro.medium.com/max/1400/1*1vwWIW5GO6DPG61479l39w.png)

![alt text](https://miro.medium.com/max/1400/1*wCnFw3EzNicaCGfA6FAMqA.png)

### results():-
- result() takes a movie's title as input and returns the top 20 recommendations using the recommend_movies() function.

## app.py
- The Flask app where we use the recommendation.py as a module and return the results in JSON format. 



# Folder
## Dataset
- Contains the dataset we have used to build our recommendation system.
