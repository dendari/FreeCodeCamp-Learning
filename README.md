# FreeCodeCamp-Learning
My solutions to the freecodecamp.com bonfires

Return the remaining elements of an array after chopping off n elements from the head.


function slasher(arr, howMany) {
   // it doesn't always pay to be first
  str = arr.slice(howMany); // slice is a function that removes from the beginning you can also add an ending object
  return str; 
}

slasher([1, 2, 3], 2);
