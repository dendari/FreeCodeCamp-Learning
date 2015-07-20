# FreeCodeCamp-Learning
My solutions to the freecodecamp.com bonfires

Return true if the string in the first element of the array contains all of the letters of the string in the second element of the array.

For example, ['hello', 'Hello'], should return true because all of the letters in the second string are present in the first, ignoring case.

The arguments ['hello', 'hey'] should return false because the string 'hello' does not contain a 'y'.

Lastly, ['Alien', 'line'], should return true because all of the letters in 'line' are present in 'Alien'.

function mutation(arr) {
  var first = arr[0].toLowerCase();
  var second = arr[1].toLowerCase(); // mutation is multidimentional so pull each element and make it lower case
  
  for(var i = 0; i < arr[1].length; i++) { // Loop the length of the second element in original array
    if(first.indexOf(second[i]) === -1) { // compare every element of second array with first array false if you don't find it
      return false;
    }
  }
  return true; // if every element from second is in the first return true
}

mutation(['hello', 'hey']);
