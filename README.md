# FreeCodeCamp-Learning
My solutions to the freecodecamp.com bonfires

Write a function that splits an array (first argument) into groups the length of size (second argument) and returns them as a multidimensional array.

function chunk(arr, size) {
  var chunkarr = [], 
      i = 0, 
      n = arr.length; // create a new array with members i and arr.length
 
  while (i < n) { // loop throgh the length of the array by 2's
    chunkarr.push(arr.slice(i, i += size));  // push elements from i to i=+size as an element of an array
  } 
 
  return chunkarr; 
}

chunk(['a', 'b', 'c', 'd'], 2);
