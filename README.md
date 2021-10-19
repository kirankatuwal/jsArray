# jsArray
Traversal of array
1) for in 
Example:
var myFriends = ['kiran','katuwal','singh'];
for (let elements in myFriends){
console.log(elements);
}

Output
0
1
2


2) For of
Example:
var myFriends = ['kiran','katuwal','singh'];
for (elements of myFriends){
console.log(elements);
}

Output
kiran
katuwal
singh


3) For Each
Example:
var myFriends = ['kiran','katuwal','singh'];
myFriends.forEach((element,index,array)=>{
console.log(element + " index : "+index+ " of array: "+array);
});

Output
kiran index : 0 of array: kiran,katuwal,singh
katuwal index : 1 of array: kiran,katuwal,singh
singh index : 2 of array: kiran,katuwal,singh

4) For loop
Example
var myFriends = ['kiran','katuwal','singh'];
for(var i = 0;i<myFriends.length; i++){
console.log(myFriends[i]);
}

Output
kiran
katuwal
singh

---------------------------
CRUD in JS
1) push -> add value to array at the last position and returns new length
Example:
var myPlants = ['broccoli', 'cauliflower', 'kale', 'tomato', 'cabbage'];
console.log(myPlants);
console.log(myPlants.push('carrot','brinjal'));
console.log(myPlants);

Output
0: "broccoli"
1: "cauliflower"
2: "kale"
3: "tomato"
4: "cabbage"
5: "carrot"
6: "brinjal"
length: 7

2) pop -> remove value to array at the last position and returns new length
Example:
var myPlants = ['broccoli', 'cauliflower', 'kale', 'tomato', 'cabbage'];
console.log(myPlants);
console.log(myPlants.pop());
console.log(myPlants);

Output
0: "broccoli"
1: "cauliflower"
2: "kale"
3: "tomato"
length: 4

3) unshift-> add value to array at the first position and returns new length
Example:
var myPlants = ['broccoli', 'cauliflower', 'kale', 'tomato', 'cabbage'];
console.log(myPlants);
console.log(myPlants.unshift('carrot','brinjal'));
console.log(myPlants);

Output
0: "carrot"
1: "brinjal"
2: "broccoli"
3: "cauliflower"
4: "kale"
5: "tomato"
6: "cabbage"
length: 7

4) shift-> remove value to array at the first position and returns new length
Example:
var myPlants = ['broccoli', 'cauliflower', 'kale', 'tomato', 'cabbage'];
console.log(myPlants);
console.log(myPlants.shift());
console.log(myPlants);

Output
0: "cauliflower"
1: "kale"
2: "tomato"
3: "cabbage"
length: 4
------------------------------------------
Find out square root of :
let arr = [25,36,49,64,81];
let sqRoot = arr.map((curElem)=> Math.sqrt(curElem) );
console.log(sqRoot);


Output
0: 5
1: 6
2: 7
3: 8
4: 9
length: 5


---------------------------------------
SOLVE THE PROBLEM with chaining method
let arr = [2,3,4,6,8];
let arr2 = arr.map((curElem)=>{
return curElem * 2;
}).filter((curElem) =>{
return curElem >10;
});

console.log(arr2);

//Making in one line 
let arr = [2,3,4,6,8];
let arr2 = arr.map((curElem)=>curElem * 2).filter((curElem) =>curElem >10);
console.log(arr2);

Output
0: 12
1: 16
length: 2
----------------------------------------
Example of reduce
let arr = [2,3,4,6,8];
let arr2 = arr.map((curElem)=>curElem * 2).filter((curElem) =>curElem >10).reduce((accumulator,curElem)=>accumulator+=curElem);
console.log(arr2);

Output
28
