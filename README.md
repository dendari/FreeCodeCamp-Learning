# FreeCodeCamp-Learning
My solutions to the freecodecamp.com bonfires

Write a function that takes two or more arrays and returns a new array of unique values in the order of the original provided arrays.

In other words, all values present from all arrays should be included in their original order, but with no duplicates in the final array.

The unique numbers should be sorted by their original order, but the final array should not be sorted in numerical order.

Check the assertion tests for examples.

function unite(arr1, arr2, arr3) {
var flattened = [arr1, arr2, arr3].reduce(function(a, b) { // flattens the three arrays into one
  return a.concat(b); 
});
  
 var tmp = [];
 
    for(var i = 0; i < flattened.length; i++){ // removes all the duplicates
        if(tmp.indexOf(flattened[i]) == -1){
        tmp.push(flattened[i]);
        }
    }
  return tmp;
}

unite([1, 2, 3], [5, 2, 1, 4], [2, 1]);
