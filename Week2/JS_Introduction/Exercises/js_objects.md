<!--Tags=["objects"]-->

# Exercises on Objects

###  Exercise 1
1. Create an object called *family* with a few properties
2. Display only the properties
3. Display only the values 

###  Exercise 2
```javascript
var building = {
    number_levels : 4,
    number_of_apt_by_level : {
        "1": 3,
        "2": 4,
        "3": 9,
        "4": 2,
    },
    name_of_tenants : ["Sarah", "Dan", "David"]
    number_of_rooms_and rent:  {
        "Sarah": [3, 2000],
        "Dan":  [4, 1000],,
        "David": [1, 10],
    },
}
```
1. Display the number of levels in the building
2. Display how many apartments are on level 1 and 3. Do the sum of these apartments
2. Display the name of the second tenant and the number of rooms he has in his apartment
3. Check if the rent of Sarah plus the rent David is bigger than the rent of Dan. 
If it is than inform the owner that he has to inscrease the rent of Dan. And change the rent of Dan accordingly inside the object.


###  Exercise 3
1. First, make a list called `myGroceries` with the values "banana","orange", and "apple".  It means you want to buy 1 item from each fruit.
2. Create this two objects: 

```javascript
var stock_in_shop= { 
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

3. Define a function called `myBill` that takes no argument. `return` the total of the expense for your groceries .
4. Call the function myBill 

Bonus: 
5. In the function above, only add the price if the item is in stock. 
* If the item is in stock, decrease the item's stock by 1

###  Exercise 4 _ **GoldExercise**
1. Create two objects, each one should hold a person details. Here are the details:  fullName, mass, height.
2. Each object should also have a propertie which value is a function that calculates the Body Mass Index (BMI) of each person
3. Create a JS function that compare both the BMI. 

