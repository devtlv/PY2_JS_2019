# Project

How it should look like (but as a list, not as a table)

> Form 
> input
> input 
> button 

Name | country | picture
--- | ---- | ----
Cow | France |  ![cow](https://www.thelocal.fr/userdata/images/article/e520a55e3f576ef9b7c24a8cbed6b42332064c193180ce853164c2e90fc3dbf6.jpg)
Dog | Great Britain |  ![dog](https://cdn.images.express.co.uk/img/dynamic/128/590x/secondary/Britain-dogs-most-likely-dumped-tragic-numbers-830186.jpg)


1. Create a form that contains:  

Two inputs 
* `class="animal_input"` 
* `class="country_input"`

One button  
* `class="post_animal"`

One section to render the data  
```html run 
<section class="animals">          
<h2>Animals</h2>          
<ul></ul>        
</section>    
```


2. Declare the `addAnimal` function that has two parameters, "name" and "country". 
3. Create an event handler for when the button is getting clicked.  This event handler has to invoke `addAnimal(x,y)` where x and y are the information typed inside the inputs. 
4. Create a global array called `animals`.  
5. Inside the addAnimal function, create a object called `newAnimal `with the keys name and country.
6. Push this object into the array `animals`  
7. Declare the function `renderAnimals` that takes no parameter. This function should append the each element of `animals`array inside the section. 
8. Where do you think the  `renderAnimals` function should be invoked  ? Then invoke it. 
9. Create the `capitalize` that take one parameter. It should return the name of the animal with the fisrt letter uppercase.
10. Where do you think the  `capitalize` function should be invoked  ? Then invoke it. 

Bonus:  we want to add pictures of the animals  
1. Create a global array called ` typeAnimals` that is a list of type of animals. 
2. Create a folder images  and download images of all the type of animals (ie typeAnimals)   
3. Create a function `addImage` that takes one parameter. This function should loop through the  `typeAnimals` array and compare the animal name (ie parameter) with the animal type (ie typeAnimals array)  •
If the comparison is correct than create a variable `imgAnimal`, and make it equal to the animal type. 
If not, the variable `imgAnimal` should be set to the string ‘"coming soon". 
Either way, return `imgAnimal`.  
4. Where do you think the  `addImage` function should be invoked  ? Then invoke it. 
