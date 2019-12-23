### <center>Project : IMDI</center>
### <center>IMDB for DevelopersInstitute</center>

#### PART 3

##### PART A : Add a poster for the film
1.	Create a new model : *Poster*
    •	image : ImageField 
    •	explanation_text 

In the model *Film*, create a relation *OneToOne* with the model *Poster*. 
--> A film can have only one poster and a poster is linked to only one film 

2.	Create a form *AddPosterForm*
3.	Edit the *AddFilmForm* in order to exclude the poster attribute 
4.	How can we add a poster to the film when we add a new film ?

![image](https://user-images.githubusercontent.com/30896388/71346448-9388c380-2570-11ea-9fa3-934127be53af.png)
