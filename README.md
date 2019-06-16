# pyflix

Django movie app on heroku
This line in the css file was giving me hard time with heroku:
/* fallback for old browsers */
	/*     background-image: url('./clock-pattern.png'); */
  
  heroku deployment error message was:
   The CSS file 'movies/app.css' references a file which could not be found:
remote:          movies/clock-pattern.png

so i deleted to see what happens. 

What we understand from this is that we can't reference files that does nor exist not even in a comment
because upperantly heroku can detect it.

You can find this movie app at https://pyflix.herokuapp.com/ 

Users can create movies and it will be stored on the database using AirTable 

It Supports full CRUD functionality by allowing users to update the movies they created 
And also delete them 

Part of the creating process users are able to rate the movies from 1-10 
rating is a required step so the movie will not be created with out ratings. 
