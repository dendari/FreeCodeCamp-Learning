# FreeCodeCamp-Learning
My solutions to the freecodecamp.com bonfires

You will be provided with an initial array (the first argument in the destroyer function), followed by one or more arguments. Remove all elements from the initial array that are of the same value as these arguments.

function destroyer(arr) {
  newArr = arr.filter(function(a) { // filter out values not in the list 
    if(a != arr[1] && a != arr[2]) { // return only values that are not the second or third argument 
      return a;
    }
  });
  return newArr;
}

destroyer([1, 2, 3, 1, 2, 3], 2, 3);
