# FreeCodeCamp-Learning
My solutions to the freecodecamp.com bonfires

Repeat a given string (first argument) n times (second argument). Return an empty string if n is a negative number.

function repeat(str, num) {
 
  if(num > 0) {
    str = str.repeat(num);  // how easy is it to repeat a string
   
  } else {
    str = ''; // if num is 0 set the string to null
  }
  return str;
}

repeat('abc', 3); 
