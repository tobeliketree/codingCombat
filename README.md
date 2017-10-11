# codingCombat



/*

frontBack
Given a string, return a new string where the first and last chars have been exchanged.

frontBack("code") → "eodc"
frontBack("a") → "a"
frontBack("ab") → "ba"

*/


function frontBack(str) {
  // return just the string if estring is 1 character or less
  if (str.length <=1) {
    return str;
  }
  // this is grabbing the middle portion of the string
  var middle = str.substring(1, str.length -1);

  // return  last letter of string + middle of string + first letter of string
  return  str.charAt(str.length -1) + middle + str.charAt(0);
}

console.log(frontBack("code"));
console.log(frontBack("a"));
console.log(frontBack("ab"));
