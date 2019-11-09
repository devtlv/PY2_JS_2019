<<<<<<< HEAD
# Solution Exercises Objects

###  Exercise 3
1. First, make a list called `myGroceries` with the values "banana","orange", and "apple". 
2. Create this two objects: 

```javascript
var stock = { 
=======
# Solution of exercises

## Exercise 3

###  Exercise 3
1. First, make a list called `myGroceries` with the values "banana","orange", and "apple".  It means you want to buy 1 item from each fruit.
2. Create this two objects: 

```javascript
var stock_in_shop= { 
>>>>>>> master
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

<<<<<<< HEAD
3. Define a function called `myBill` that takes no argument. `return` the total of the expense for your groceries  
=======
3. Define a function called `myBill` that takes no argument. `return` the total of the expense for your groceries .
>>>>>>> master
4. Call the function myBill 

Bonus: 
5. In the function above, only add the price if the item is in stock. 
* If the item is in stock, decrease the item's stock by 1

<<<<<<< HEAD
### Solution
``` javascript
var somme =0;

function myBill(){
=======
## Solution

```javascript
var somme =0;
function myBill(){
    
>>>>>>> master
    for(var property in stock){
        if (stock[property]>0){
            somme+= prices[property];
            stock[property]-=1;
            console.log(stock[property]);
        }
    }
<<<<<<< HEAD

}
myBill();
```


=======
    return somme;
}

myBill()
```
>>>>>>> master

###  Exercise 4 _ **GoldExercise**
1. Create two objects, each one should hold a person details. Here are the details:  fullName, mass, height.
2. Each object should also have a propertie which value is a function that calculates the Body Mass Index (BMI) of each person
3. Create a JS function that compare both the BMI. 


<<<<<<< HEAD
### Solution
``` javascript
 var person_1= {
        fullName:"bob saggit",
        mass:70, 
        height:175,
        bmi: ()=>
=======
## Solution

```javascript
ar person_1= {
        fullName:"bob saggit",
        mass:70, 
        height:175,
        bmi: () =>
>>>>>>> master
            parseInt(this.mass)/(parseInt(this.height)**2)
        
    }
​
var person_2= {
        fullName:"mic jagger",
        mass:90, 
        height:180,
        bmi: ()=>
            parseInt(this.mass)/(parseInt(this.height)**2)
        
    }
​
function comp_bmi() {
    if((person_1.bmi()) > (person_2.bmi())){
        console.log(person_1.fullName + " is heavier")
    }
    else if((person_1.bmi()) < (person_2.bmi())){
        console.log(person_2.fullName + " is heavier")
    }
    else{
        console.log(person_1.fullName + "" +person_2.fullName+" are the same")
    }
}
<<<<<<< HEAD
```
=======

```
>>>>>>> master
