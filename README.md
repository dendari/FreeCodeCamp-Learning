# FreeCodeCamp-Learning
My solutions to the freecodecamp.com bonfires

Compare two arrays and return a new array with any items not found in both of the original arrays.

function diff(arr1, arr2) {
  var newArr = [];
  
  arr1.forEach(function(number){ //forEach loops through each element in the array
    if(arr2.indexOf(number) === -1){ // checking if each element of arr[1] is in arr[2] and pushing it to newArr 
      newArr.push(number);
    }
  });
  
  arr2.forEach(function(number){ 
    if(arr1.indexOf(number) === -1){ // checking if each element of arr[2] is in arr[1] and pushing it to newArr
      newArr.push(number);
    }
  });
  // Same, same; but different.
  return newArr;
}

diff([1, 2, 3, 5], [1, 2, 3, 4, 5]);
