### <center>Project : IMDI</center>
### <center>IMDB for DevelopersInstitute</center>

#### PART 2

##### PART A: film_app : Add a film and a director

1.	Create 4 new models :
    1.	Country : 
             •	name
    2.	Category : 
            •	name
    3.	Film: 
            •	title
            •	release_date (default the date of today) 
            •	country : ForeignKey of Country
            •	category: ForeignKey of Category
    4.	Director: 
            •	first_name
            •	last_name
            •	film : ForeignKey of Film

2.	Create the forms : *AddFilmForm* and *AddDirectorForm*
3.	Create the routes : *addFilm* and *addDirector*
4.	Create the functions : *addFilm* and *addDirector*
5.	In templates, create a folder *director* with the file *addDirector.html*
6.	In templates, create a folder *film* with the file *addFilm.html*
7.	The new films with their director have to render on the template *homepage*. You have to use the component card of Bootstrap to style the page.

![image](https://user-images.githubusercontent.com/30896388/71343769-73093b00-2569-11ea-8776-0c26f56461c8.png)

8. Be careful, the date has to be in “human” format.
9.  The routes *addFilm*  and *addDirector* have to render in the navbar of homepage, **only if the user is a superuser.**

![image](https://user-images.githubusercontent.com/30896388/71343812-92a06380-2569-11ea-8e88-bc1dbc20e7cd.png)

![image](https://user-images.githubusercontent.com/30896388/71343821-9a600800-2569-11ea-907d-dfc214b31c73.png)




