```
function findLongestWordLength(str) {

  let myArray = [];
  let count = 0;
  
  //Break array into pieces
  myArray = str.split(" ");
 
  for(let i = 0; i < myArray.length; i++)
  {
    //Check if the current array element is greater than the current count
    //If it is, update count with new length
    if(myArray[i].length > count){
      count = myArray[i].length;
    }
  }
  //When done, return the largest count
  return count;
}

findLongestWordLength("The quick brown fox jumped over the lazy dog");
```
