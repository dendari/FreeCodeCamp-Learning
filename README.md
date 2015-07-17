# FreeCodeCamp-Learning
My solutions to the freecodecamp.com bonfires

Return the provided string with the first letter of each word capitalized.

For the purpose of this exercise, you should also capitalize connecting words like 'the' and 'of'.

function titleCase(str) {
  // replace word followed by white space with the function that makes character 0 uppercase and makes all the other letters lower case
str = str.replace(/\w\S*/g, function(txt){return txt.charAt(0).toUpperCase() + txt.substr(1).toLowerCase();});
  
  return str;
  
}

titleCase("I'm a little tea pot");
