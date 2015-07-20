# FreeCodeCamp-Learning
My solutions to the freecodecamp.com bonfires

Make a function that looks through a list (first argument) and returns an array of all objects that have equivalent property values (second argument).

function where(collection, source) { 
  var arr = [];
  for(var i = 0; i < collection.length; i++){
    if(collection[i].last === source.last){ // check to see if the object in souce labled last is also in collections
      arr.push(collection[i]); // If it is add it to var arr
    }
  }
  // What's in a name?
  return arr; // return all elements that are in both lists
}

where([{ first: 'Romeo', last: 'Montague' }, { first: 'Mercutio', last: null }, { first: 'Tybalt', last: 'Capulet' }], { last: 'Capulet' });
