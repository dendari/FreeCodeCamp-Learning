# FreeCodeCamp-Learning
My solutions to the freecodecamp.com bonfires

Remove all falsey values from an array.

Falsey values in javascript are false, null, 0, "", undefined, and NaN.

function bouncer(arr) {
  // Don't show a false ID to this bouncer.
  var b = arr.filter(Boolean); // filter removes all Boolean values from the array
  return b;
}

bouncer([7, 'ate', '', false, 9]);
