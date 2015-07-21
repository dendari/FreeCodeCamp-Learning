# FreeCodeCamp-Learning
My solutions to the freecodecamp.com bonfires

Return the sum of all odd Fibonacci numbers up to and including the passed number if it is a Fibonacci number.

The first few numbers of the Fibonacci sequence are 1, 1, 2, 3, 5 and 8, and each subsequent number is the sum of the previous two numbers.

As an example, passing 4 to the function should return 5 because all the odd Fibonacci numbers under 4 are 1, 1, and 3.

function sumFibs(num) {
  var fibs = [1,1]; // a bit of a cheat
  
  for(var i=2; i<num; i++){ // already have the first two numbers
     fibs[i] = (fibs[i-1] + fibs[i-2]);  // the ith number is the sum of the previous two
   } 

  var answer = 0;
  for(var j = 0; j < num; j++) {
    if(fibs[j]%2 !== 0 && fibs[j] <= num){ // checking for odd and keeping below top num
      answer += fibs[j]; // adding all the numbers
    } 
  }
   return answer;
}
sumFibs(4);
