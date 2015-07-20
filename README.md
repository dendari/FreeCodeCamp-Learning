# FreeCodeCamp-Learning
My solutions to the freecodecamp.com bonfires

Convert a string to spinal case. Spinal case is all-lowercase-words-joined-by-dashes.

function spinalCase(str) {
// Search using regex add a space before capitals add replace space and underscore with hypen and then convert everything to lowercase
  return str.replace(/([a-z](?=[A-Z]))/g, '$1 ').replace(/\W/, '-').replace(/\s|\_/g , "-").toLowerCase();
}

spinalCase('This Is Spinal Tap');
