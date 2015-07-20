# FreeCodeCamp-Learning
My solutions to the freecodecamp.com bonfires

Find the missing letter in the passed letter range and return it.

If all letters are present in the range, return undefined.

function fearNotLetter(str) {
 for (var i = 0; i < str.length - 1; i++) {
        if (str.charCodeAt(i + 1) - str.charCodeAt(i) != 1) { //charCodeAt()  of 2 letters in a row are sequential so subtracting them should equal 1, if it isn't then return what should be the next number in line. 
            return String.fromCharCode(str.charCodeAt(i) + 1);
        }
    }
}

fearNotLetter('abce');
