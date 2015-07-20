# FreeCodeCamp-Learning
My solutions to the freecodecamp.com bonfires

Convert the characters "&", "<", ">", '"' (double quote), and "'" (apostrophe), in a string to their corresponding HTML entities.

function convert(str) {
// serach through regex and replace with HTML equivalent when found
  str = str.replace(/&/g, "&amp;").replace(/>/g, "&gt;").replace(/</g, "&lt;").replace(/"/g, "&quot;").replace(/'/g, "&apos;"); 
  return str;
}
convert('Dolce & Gabbana');
