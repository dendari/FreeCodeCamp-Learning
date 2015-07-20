# FreeCodeCamp-Learning
My solutions to the freecodecamp.com bonfires

Convert the given number into a roman numeral.

All roman numerals answers should be provided in upper-case.

function convert(num) {

  if(num < 1){ return "";}  // basically keeps running all the if statements until num reaches 0
  if(num >= 40){ return "XL" + convert(num - 40);}  // if num >= 40 print XL then subtract 40
  if(num >= 10){ return "X" + convert(num - 10);}  // if num >= 10 print X then subtract 10 prints 3 X's
  if(num >= 9){ return "IX" + convert(num - 9);} // if num >= 9 print IX then subtract 9
  if(num >= 5){ return "V" + convert(num - 5);} // if num >= 5 print V then subtract 5
  if(num >= 4){ return "IV" + convert(num - 4);} // if num >= 4 print IV then subtract 4
  if(num >= 1){ return "I" + convert(num - 1);}  // if num >= I print I then subtract 1
  // this only works on numbers up to 40 but could be easily expanded 
}

convert(36);
