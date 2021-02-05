# Find the Longest Word in a StringPassed

###
Return the length of the longest word in the provided sentence.

Your response should be a number.

### Solution

```javascript
function findLongestWordLength(str) {
  //Spliting the string
  let x = str.split(' ');
  let lWord = 0;
  for(let i = 0; i < x.length;i++){
     if(lWord < x[i].length){
        lWord = x[i].length;
     }
  }
  console.log(lWord);

  return lWord;
}

findLongestWordLength("The quick brown fox jumped over the lazy dog");
```
