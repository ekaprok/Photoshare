# Photoshare
###Photoshare is a database system for a web based photo social sharing application written in MySQL and Python Flask. 

The system has the following interactions:
####(1) User and Friends Management: 
	Every User has the following attributes: first name, last name, email, date of birth, hometown, gender, and password. Anyone can register if the email is unique for the database. And every user can have multiple friends. Any registered user can find a friend by typing a person’s email. 

####(2) Albums and Photos Management:
	Any user can add any number of albums. However, a user cannot have two albums with the same name (albumName and uid are unique). Users can delete albums and photos. When an album is deleted, all the photos it contains are also deleted. 
Any visitor of the website can see all the photos. 

####(3) Comments and Likes:
	Any user and visitor of the website can leave comments and likes to the pictures on the home page (hello.html).

####(4) Tags:
	A logged in user can leave tags for each photo. Tags provide a way to categorize photos and each photo can have any number of tags. A user can also click on the tag and see all the photos associated with the user’s photos and all the photos on the website. One can also see the most popular tags that are listed in the bottom of hello.html page. Also, visitors and users can search for pictures using one or more tags.

####(5) Recommendations:
	Every user can see recommended photos on profile.html page. The functionality is achieved by the following way: take the five most commonly used tags among the user's photos. Perform a disjunctive search through all the photos for these five tags. A photo that contains all five tags should be ranked higher than one that contained four of the tags and so on. 


####(6) User Activity:
	userActivity() method finds the most active users according to the number of comments they post. The results can be found on the profile page.
  
