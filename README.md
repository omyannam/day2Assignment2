# day2Assignment2
LetsUpgrade
Question 1:
Write a JS code which takes input from the user
 and logs it in the console.
Answer :-



<script> 
console.log("Hello"); 
</script> 







Question 2:
Explain with examples the remaining methods of 
String and Array
Answer :-
Array Methods:
_____________
If we want to represents multiple elements in a single variable, then we can go with an array.
var a=[10,20,30,10]
In array we can insert duplicate elements.
Through indexes, we can retrive an elements from array.
Array index, always starts with 0.
Ex:

var array=[10,20,30];
console.log(array[0]);
Result: 10
console.log(array[2]);
Result: 30

length

length property is used to get the length of an array.
Ex:

var array=[10,20,30];
console.log(array.length);
Result: 3

push(---)

push(---) is used to insert an element(s) in the last index.
Ex:

var array=[10,20,30];
array.push(40);
Result: [10,20,30,40]
array.push(50,60,70);
Result: [10,20,30,40,50,60,70]

Return type: number(new length of array);

pop()

pop() used to remove an element from last index.
Ex:

var array=[10,20,30];
array.pop()
Result: 30

Return last element.

unshift(---)

unshift(---) is used to insert an element(s) in the first index.
Ex:

var array=[10,20,30];
array.unshift(40);
Result: [40,10,20,30]
array.unshift(50,60,70);
Result: [50,60,70,40,50,60,70]

Return type: number(new length of array);

shift()

shift() used to remove an element from first index.
Ex:

var array=[10,20,30];
array.shift()
Result: 10

Return first element.

indexOf(-)

indexOf(-) , it gives an index of element in the array.
It take one arguement.
Using indexOf(), we can check one element is there or not in the array. If there it return that element index, if not it returns -1.
Ex:

var array=[10,20,30];
array.indexOf(20)
Result: 1
array.indexOf(200)
Result: -1
array.indexOf(30)
Result: 2
array.indexOf(120)
Result: -1

Note: If you observe above one, if the element is there it return the index of the element, if not there, it always returns -1.

Return type: number.

lastIndexOf(-)

lastIndexOf(-) , it gives last matching element index, in the array.
It take one arguement.
Ex:

var array=[10,20,30,20,10,20];
array.lastIndexOf(20)
Result: 5
array.lastIndexOf(200)
Result: -1
array.lastIndexOf(30)
Result: 2

Return type: number.

includes(-)

Using includes(), we can check one element is there or not in the array. If there it return true, if not it returns false.
It take one arguement.
Ex:

var array=[10,20,30];
array.includes(20)
Result: true
array.includes(200)
Result: false
array.includes(30)
Result: true
array.includes(120)
Result: false

Note: If you observe above one, if the element is there it returns true, if not it returns false.

Return type: boolean.

join(-)

join(-) , which is used to convert array into string with some delemeter.
Default delemeter is ','.
Ex:

var array=[10,20,30];
array.join()
Result:"10,20,30"
array.join('_')
Result: "10_20_30"

Return type: string.

reverse()

reverse() , which is used print an array in the reverse order.
Ex:

var array=[10,20,30];
array.reverse()
Result:[30,20,10]

Return type: array.

concat(---)

concat(---), which is used to combine two arrays.
It creates new result array.It's not effect the original array.
Ex:

var array=[10,20,30];
array.concat(40,50)
Result: new Array create with this data[10,20,30,40,50]

Return type: array.

forEach(-)

forEach(-), which is used to retrive data from array.
Which take one callback function as an arguement.
The call back function has two arguements, value ,index.
Ex:

var array=[10,20,30];
array.forEach(function(value,index)}
console.log(value);
})

every(-)

every(-), which is used to check array elements based on condition, which return boolean value.
If all elements in the array,satisfied your condtion then returns true.
If minimum one element in the array, is not satisfied your condtion then returns false.
Ex:

var array=[10,20,30];
array.every(function(value,index)}
return value > 5
})
Result: true
array.every(function(value,index)}
return value > 15
})
Result: false

some(-)

some(-), which is used to check array elements based on condition, which return boolean value.
If minimum one element in the array, is satisfied your condtion then returns true.
If no element in the array, is not satisfied your condtion then returns false.
Ex:

var array=[10,20,30];
array.some(function(value,index)}
return value > 15
})
Result: true
array.some(function(value,index)}
return value > 50
})
Result: false









String Methods:
var name="sachin";

length

length property is used to get the length of string.
Ex:

var name="sachin"
console.log(name.length);
Result: 6

indexOf(-)

indexOf(-) , it gives an starting index of charactor(s) in the string.
It take one arguement.
Using indexOf(), we can check charactor(s) is there or not in the string. If there it return that charactor(s) starting index, if not it returns -1.
Ex:

var name="sachin";
name.indexOf('ch')
Result: 2
name.indexOf('z')
Result: -1

Note: If you observe above one, if the charactor(s) is there it return that starting index of the charactor(s), if not there, it always returns -1.

Return type: number.

lastIndexOf(-)

lastIndexOf(-) , it gives last matching charactor(s) index, in the string.
It take one arguement.
Ex:

var name="sachin tendulkar";
name.lastIndexOf('a')
Result: 14

Return type: number.

includes(-)

Using includes(), we can check charactor(s) is there or not in the string. If there it return true, if not it returns false.
It take one arguement.
Ex:

var name="sachin";
name.includes('ch')
Result: true
name.includes('z')
Result: false

Note: If you observe above one, if the charactor(s) there it returns true, if not it returns false.

Return type: boolean.

chartAt(-)

chartAt(-) ,which gives the charactor at that positions.
Ex:

var name="sachin";
name.charAt(2); Result: c

charCodeAt(-)

charCodeAt(-) ,which gives the ASCII value of charactor at that positions.
Ex:

var name="sachin";
name.charCodeAt(2); Result:115

startsWith(-)

startsWith(-) ,which is used to check that string is starts with given charactor(s).
It returns boolean value
It check for case sensitive.
Ex:

var name="sachin";
name.startsWith('sa'); Result:true
var name="sachin";
name.startsWith('Sa'); Result:false

endsWith(-)

endsWith(-) ,which is used to check that string is ends with given charactor(s).
It returns boolean value
It check for case sensitive.
Ex:

var name="sachin";
name.endsWith('in'); Result:true
var name="sachin";
name.endsWith('In'); Result:false

concat(--)

concat(--), which is used to combine two strings.
Ex:

var name1="sachin"; var name2="dhoni"; var result=name1.concat(name2); console.log(result); Result: sachindhoni

slice(-,-)

slice(-,-), which is used to get the part of a string
slice(-,-), take 2 arguements, whose types are number.
First arguement represents your starting index, from there we can take n(difference of first and second arguement) charactor(s).
In slice method, first arguement always less than second arguement.
Ex:

var name='sachin'
name.slice(1,3)
Result:"ac"
name.slice(3,1)
Result:""

substring(-,-)

substring(-,-), which is used to get the part of a string
substring(-,-), take 2 arguements, whose types are number.
First arguement represents your starting index, from there we can take n(difference of first and second arguement) charactor(s).
Ex:

var name='sachin'
name.substring(1,3)
Result:"ac"
name.substring(3,1)
Result:"ac"

substr(-,-)

substr(-,-), which is used to get the part of a string
substr(-,-), take 2 arguements, whose types are number.
First arguement represents your starting index, from there we can take n(second arguement) charactor(s).
Ex:

var name='sachin'
name.substr(1,3)
Result:"ach"

toUpperCase()

toUpperCase(), which is used to convert your string into uppercase letters.
Ex:

var name='sachin'
name.toUpperCase()
Result:"SACHIN"

toLowerCase()

toUpperCase(), which is used to convert your string into lowercase letters.
Ex:

var name='SACHIN'
name.toLowerCase()
Result:"sachin"








Question 3:
Ask the user if he is 21+ and log the value "Can drink"
, "Cannot Drink"
Answer :-
<script>
let a;
if (a==21+)
{
console.log("can drink")
}
else
{
console.log("Cannot Drink")
}

</script>
























