# FreeCodeCamp-Learning
My solutions to the freecodecamp.com bonfires

Return the lowest index at which a value (second argument) should be inserted into a sorted array (first argument).

For example, where([1,2,3,4], 1.5) should return 1 because it is greater than 1 (0th index), but less than 2 (1st index).

function where(arr, num) {
  arr = arr.sort(); // sort the array by unicode order
  for(var i = 0; i < arr.length; i++){
     if(num > arr[i] && num <= arr[i+1]){ // find the spot where num is greater than an element but less or equal to the next
       return i+1; // return where it would be inserted 
     }
  }
}

where([40, 60], 50);
