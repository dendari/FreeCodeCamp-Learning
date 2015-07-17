# FreeCodeCamp-Learning
My solutions to the freecodecamp.com bonfires

Check if a string (first argument) ends with the given target string (second argument).

function end(str, target) {
// delete the length of the string minus the length of the target and compare it to the target
  str = str.substring(str.length-target.length) == target;
  return str;
}

end('Bastian', 'n');
