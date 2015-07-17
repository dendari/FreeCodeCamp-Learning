# FreeCodeCamp-Learning
My solutions to the freecodecamp.com bonfires

A palindrome is a word or sentence that's spelled the same way both forward and backward, ignoring punctuation, case, and spacing.

You'll need to remove punctuation and turn everything lower case in order to check for palindromes.

We'll pass strings with varying formats, such as "racecar", "RaceCar", and "race CAR" among others.

function palindrome(str) {
  str = str.toLowerCase();  // this could also be toUpperCase() just as long as everything is the same
  str = str.replace(/([\W])/g, ""); // My partner did this but I think it replaces any nonword char with a space
  
  if(str == str.split('').reverse().join('')){ // split reverse put back together and compare 
  return true;
  } else {
    return false;
  }
}



palindrome("eye");
