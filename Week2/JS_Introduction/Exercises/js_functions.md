<!---Taggs=["functions"]--->

# Exercises functions

## Exercise 1
1. Write a JS function that takes a parameter: myAge
2. Display the name of my mum and my dad (my mum is twice my age, and my dad is 1.2 the age of my mum)

 
## Exercise 2
Let's create functions that calculate your vacation’s costs: 

1. Define a function called `hotel_cost`, that takes one argument *nights*. This argument is an input. 
The hotel costs $140 per night.  The function should `return` the price of the hotel for the nights. 

2. Define a function called `plane_ride_cost` that takes one argument *city*. This argument is an input. 
The function should `return`a different price depending on the location. 
    "London": 183$ 
    "Paris": 220$ 
    All other destination : 300$ 
If the user answer is undefined, ask him again.

3. Define a function called `rental_car_cost` that takes one argument *days*. This argument is an input. 
Calculate the cost of renting the car:  
Every day you rent the car costs $40.

* If you rent the car for 7 or more days, you get $50 discount on your total. 
* If you rent the car for 3 to 7 days, you get $20 off your total. 
`return` that cost. 

4. Define a function called `trip_cost` that takes three arguments,*city*, *nights* and *days*.  
The function has to `return` the total cost of the vacation by calling the 3 functions defined above. 
 
> Example : The car cost: $x, the hotel cost: $y, the plane tickets cost: $z. 
 
5. Call the function `trip_cost` 

## Exercise 4 XP-GOLD
1. First, make a list called `myGroceries` with the values "banana","orange", and "apple". 
2. Create this two objects: 

```javascript
var stock = { 
    "banana": 6, 
    "apple": 0, 
    "orange": 32 
}  

var prices = {    
     "banana": 4, 
    "apple": 2, 
    "orange": 1.5 
} 
```

3. Define a function called `myBill` that takes no argument. `return` the total of the expense for your groceries  
4. Call the function myBill 

Bonus: 
5. In the function above, only add the price if the item is in stock. 
* If the item is in stock, decrease the item's stock by 1

 
## Exercise 5
1. Write a JS function that takes a list and returns a new list with unique elements of the first list.  
> Example list=[1,2,3,3,3,3,4,5] newList = [1,2,3,4,5]  
> Example list=[1,2,3,3,3,3,4,5] newList = [1,2,3,4,5]  
