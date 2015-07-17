# FreeCodeCamp-Learning
My solutions to the freecodecamp.com bonfires

Return the length of the longest word in the provided sentence.

Your response should be a number.

function findLongestWord(str) {
  str = str.split(" "); // split string into individual words
    var longest = 0;
    
    for (var i = 0; i < str.length - 1; i++) {
        if (longest < str[i].length) {
            longest = str[i].length; // Compare each word one at a time always keeping the longest
    }
  }
  return longest;
}

findLongestWord('The quick brown fox jumped over the lazy dog');
