# javascriptQuestionsAnswer


## 1.   what is Difference between var,let and const?
-  const and let variable cannot be redeclered the variable and var variable can be redeclere.
-  let and var variable can be change the value of variable and const variable cannot be change the value of varibale.
-  let and const variable can be access the inside a block but cannot be accesee the outside a block and var variable can be access the outside and inside a block.




## 2.  difference between call,apply and bind method()?

- call method has invoked the function and allows you to pass arguments one by one.
- apply method is invoked the function and its allows you to pass arguments as a array.
- bind method is return a new function and its allows you to pass arguments as a array and any number of argumnets.


example-

var obj={
	num:2
}

var add=function(a,b)//add function 
{
	console.log(this.num+a+b);
}

add.call(obj,2,1);//call

var args=[3,1];
add.apply(obj,args);//apply

var bond=add.bind(obj);//returns to another function==>bind
bond(4,1);

output=>5
6
7
 
 
 ## 3.what is an array?
The array is a collection of similar data types but in javascript, we can store the different types of array elements.

let a1=[1,2,3,"abc"];
console.log(a1);

output->1,2,3,abc

## 4.Difference between splice() and slice() in javascript?
 slice does not modify the original array.

- let a=[3,4,5,6,7];
- var arr=a.slice(0,2);
- console.log(arr);//3,4
- console.log(a);//3,4,5,6,7

splice modify the original array.

- let array=[1,2,3,4,5];
- var array1=array.splice(0,2,"ABBCC");
- console.log(array1);//1,2
- console.log(array);//"ABBCC",3,4,5

2)slice is used to pick the elements from an array. and a splice is used to delete and insert elements to the array

## 5. what is the object of javascript?
In javascript there are 8 data types first seven data types are primitive datatypes because these datatypes contain a single value but the object data types contain a collection of various data
the object can be created with brackets and a list of properties. A property is a key-value pair
the given key is a name of property it is defined as a string and value can be anything


## 6. what are the map of javascript?
The map is a collection of keyed data items just like an object.

- new map()=>its a created a new map.
- map. set(key,value)->store the value by key.
- map. get(key)->get the value by the key.
- map .has(key)->return true if the given key exists otherwise false
- map. delete(key)->removes the value of a key.
- map .clear(key)->clear everything from map.
- map.size->returns current elements of count

## 7. what is set in javascript?
A set is a collection of special value. each value may occur only once.

- let m=new Set();
- m.add(1);
- m.add(1);
- m.add(3);

- for (let user of m)
- 	console.log(user);//1,3

## 8. Difference between map and object?
#### objects are similar to maps in that both you set keys to value, retrieve those values, delete values

1) The keys on objects are string, symbol, the integer on the maps keys are object, array, function.

2) Maps contain the order of keys but the object is an unordered key

3) You can get the size of the map easily with the size property but the object can be determined manually

4) Map inherits the object which means you can technically use the object prototype function on the map but with an object, you can not use the map function











