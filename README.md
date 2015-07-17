# FreeCodeCamp-Learning
My solutions to the freecodecamp.com bonfires

Return an array consisting of the largest number from each provided sub-array. For simplicity, the provided array will contain exactly 4 sub-arrays.

Remember, you can iterate through an array with a simple for loop, and access each member with array syntax arr[i] .

If you are writing your own Chai.js tests, be sure to use a deep equal statement instead of an equal statement when comparing arrays.

function largestOfFour(arr) {
  
  var max = 0;
  var newArray = []; 
  for(var i = 0; i < 4; i++) { // loop through the 4 memebers of the array
    for(var j = 0; j < 4; j++) { // each memeber also has 4 memebers
      if (max < arr[i][j]) {
            max = arr[i][j]; // set max to the max number within the multidimentional array
       } 
      
    } 
    newArray.push(max); // push the max number into a new array
  }
  
   return newArray;
}

largestOfFour([[4, 5, 1, 3], [13, 27, 18, 26], [32, 35, 37, 39], [1000, 1001, 857, 1]]); 
