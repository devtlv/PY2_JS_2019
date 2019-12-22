### Project : IMDI
### IMDB for DevelopersInstitute

#### PART 1

1.	Create a new Django project called **film_project**
2.	Create two app : **film_app** et **account_app**

##### PART A : Account_app
1. Create 4 new routes : 
    1.	signup
    2.	login
    3.	logout
    4.	profile, that takes the id of the user as a parameter 

2.	Create 2 new forms from the User model (django_auth)
1.	SignupForm : 
    •	Username
    •	Password
    •	Email
    •	First_name
    •	Last_name

2.	LoginForm : 
    •	Username
    •	Password

3.	Create three new templates (html file) : 
    1.	login.html : renders the form LoginForm
    2.	signup.html : renders the form SignupForm
    3.	profile.html 
        •	includes the file navbar_homepage.html (**see Part B**)
        •	renders username, first_name and last_name of the user

4.	Create a function signup :
    •	Fetches the data of the form 
    •	Creates a new user 
    •	Fetches the user thanks to the method authenticate(). (For more information on the method authenticate : [documentation Django](https://docs.djangoproject.com/fr/2.1/topics/auth/default/): 
        •	If the user already exists : 
        - Connect the user (use the login method)
        - Redirect the user to the route homepage of  film_app **(see Part B**)

5.	Create a function *login* that acts like the function signup
6.	Create a function *logout*  that logouts the user and redirect him to the route index of film_app (**see Part B**) (use the method logout [documentation Django](https://docs.djangoproject.com/fr/2.1/topics/auth/default/))
7.	Create a function *profile*  that fetches and renders the user depending on his id 


##### PART B : Film_app

1.	Create two routes: `index` and `homepage`, that each renders :  index.html and homepage.html
2.	In the folder templates, create in a folder called **partials**, 4 files html in  : 
    1.	head.html : that contains the Bootstrap link and the title 
    2.	footer.html : that inherits from head.html, with the title « footer », and that contains a Bootstrap footer.
    3.	navbar_homepage.html
    4.	navbar_index.html

###### navbar_homepage.html
1. If the user is authenticated, this is what he should see in *homepage.html*
![navbar_homepage.html](https://user-images.githubusercontent.com/30896388/71320344-b5237580-24b2-11ea-8da0-384857282e2e.png)

2.	If the user is not authenticated, this is what he should see in *homepage.html*
![navbar_homepage.html](https://user-images.githubusercontent.com/30896388/71320353-ccfaf980-24b2-11ea-9cbb-e45944f4a084.png)

###### navbar_index.html
1.	If the user is authenticated, this is what he should see in *index.html*
![navbar_homepage.html](https://user-images.githubusercontent.com/30896388/71320365-f87de400-24b2-11ea-9630-a26a275d4a11.png)

2.	If the user is not authenticated, this is what he should see in index.html
![navbar_index.html](https://user-images.githubusercontent.com/30896388/71320376-121f2b80-24b3-11ea-9a19-719a30a3892d.png)






