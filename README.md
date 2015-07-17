# FreeCodeCamp-Learning
My solutions to the freecodecamp.com bonfires

Truncate a string (first argument) if it is longer than the given maximum string length (second argument). Return the truncated string with a '...' ending.

Note that the three dots at the end add to the string length.

function truncate(str, num) {
   if(str.length > num){ // if the length is > num don't do anything
  return str.slice(0,num-3) + "..."; // Cut the string 3 less than num then add the 3 dots
  } else {
  return str;
  }
}

truncate('A-tisket a-tasket A green and yellow basket', 11);
