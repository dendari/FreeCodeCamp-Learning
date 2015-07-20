# FreeCodeCamp-Learning
My solutions to the freecodecamp.com bonfires

Translate the provided string to pig latin.

Pig Latin takes the first consonant (or consonant cluster) of an English word, moves it to the end of the word and suffixes an "ay".

If a word begins with a vowel you just add "way" to the end.

function translate(str) {
 var a = [];
  if(str[0].match(/[aeiou]/i)){ // check for vowel and just add way to the end
      return str + 'way';
  } else {
    vowelindex = str.search(/[aeiou]/i); // set length to 1st vowel to end of word
    first = str.substr(0, vowelindex); //  Grab letters up until the first vowel 
    rest = str.substr(vowelindex);  // grab letter after the first vowle 
    return rest + first + 'ay'; // put everything together and add ay at the end
  }
}
translate("consonant");
