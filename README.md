# FreeCodeCamp-Learning
My solutions to the freecodecamp.com bonfires

Check if a value is classified as a boolean primitive. Return true or false.

Boolean primitives are true and false.

function boo(bool) {
  // What is the new fad diet for ghost developers? The Boolean.
   return typeof bool === 'boolean'; // typeof checks the type in this case if it is boolean
}

boo(null);
