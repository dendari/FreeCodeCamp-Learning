# FreeCodeCamp-Learning
My solutions to the freecodecamp.com bonfires

We'll pass you an array of two numbers. Return the sum of those two numbers and all numbers between them.

The lowest number will not always come first.

function sumAll(arr) {
  var a = 0;
  var min = Math.min(arr[0],arr[1]); // set the min to the smallest number
  var max = Math.max(arr[0], arr[1]); // set the max to the largest number
  
  for(var i = min; i <= max; i++){
    a += i; // set a equal to the min and add each number until you get to the max
  }
  return a;
}

sumAll([1, 4]);
