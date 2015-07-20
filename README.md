# FreeCodeCamp-Learning
My solutions to the freecodecamp.com bonfires

The DNA strand is missing the pairing element. Match each character with the missing element and return the results as a 2d array.

Base pairs are a pair of AT and CG. Match the missing element to the provided character.

Return the provided character as the first element in each array.

function pair(str) {
  arr = [];
  for(var i in str) {
    switch(str[i]) {
      case 'A': 
        arr.push(["A", 'T']); // When you find an A make a string with A,T
        break;
      case 'T':
        arr.push(['T', 'A']); // When you find a T make a string with T,A
        break;
      case 'C':
        arr.push(['C', 'G']); // When you find a C make a string with C,G
        break;
      case 'G':
        arr.push(['G', 'C']); // When you find a G make a string with G,C
        break;
    }
  }
 return arr;
}

pair("GCG");
