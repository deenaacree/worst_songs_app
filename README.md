# The Worst Songs App — A Python application 
A fully functional python application of a list of the worst songs ever. Includes Bootstrap and an embedded YouTube player for each song. 

LINK to the application, hosted at PythonAnywhere: [Worst Songs App](http://dacree.pythonanywhere.com/)


## Origins

For my final project, I wanted to create a web app that extends the small Flask app that I built for a previous assignment. That app, a simple list of songs considered the worst from Wikipedia, was something that was interesting for me to build—I added to the information already included on the list a link to a YouTube video of each song so that there was more information than just what was available on the list. 

As part of my final project, I wanted to incorporate a more attractive UI (using Bootstrap) and to extend this simple list to a functioning web app with an embedded YouTube player. 

As far as usefulness for others, I believe that this app is useful and interesting to others because:
-	It isn’t something that currently exists (the Wikipedia list could certainly be longer). 
-	Incorporating the YouTube links makes the app even more useful than a simple list. 
-	Including the option to add to the list in the app (#1 on my additional tasks list) would ensure that it will grow beyond being just 22 items.


## Goal and Technologies

#### Final Goal
At the end of my project, I want to have a fully functional and interactive web app. For the purposes of this project, I am looking to have an app that uses a Python dictionary to retrieve information about a song title, artist's name, year released, information about why the song is included on the "worst songs ever" list, and an embedded YouTube video. 

#### Technologies Required
As part of my final project, this app will include: 
-	*Python*: since the app will be made with Flask, Python is of course included. 
-	*Flask*: currently, I already have a basic Flask app. I plan to incorporate the already existing app, adding to what currently exists and making it more visually appealing.
-	*Data storage*: I have decided that I would prefer to keep the data stored in a Python dictionary instead of building a SQL database to go along with the app. Instead, I will include a form to submit more entries, which I can approve individually (I don’t anticipate there being many entries). 
-	*Bootstrap*: the web form and other parts of the website will be styled with Bootstrap so that I can spend less time on styling and more time making everything work. 
In addition, as part of each song’s page or section, my app will have an embedded YouTube player that takes the link for each song and displays the appropriate video. 


## Problems
The **only problem** that I was completely unable to fix with this project was fixing an error caused by the question mark in the song title "Who Let the Dogs Out?" This error was caused by the browser interpreting the question mark in the URL as a query. I was unable to fix this error, and because I did not want to change the way that my URL was styled, I was forced to simply remove the question mark. This was not ideal, but it was the only solution to the problem.

A big problem that I was not expecting to have was with the way that YouTube styles its embedding links. I was expecting to be able to simply find code that allowed me to use the links I had already collected and use them to embed the videos, but I was wrong. Instead, I had to go to each video, change the YouTube link in my Python dictionary, and then use the new link as a variable in the embedding code. 
