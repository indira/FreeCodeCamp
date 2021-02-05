# Intermediate Algorithm Scripting: Diff Two ArraysPassed

### 

Compare two arrays and return a new array with any items only found in one of the two given arrays, but not both. In other words, return the symmetric difference of the two arrays.

Note
You can return the array with its elements in any order.

### Original

```javascript
function diffArray(arr1, arr2) {
  var newArr = [];
  return newArr;
}

diffArray([1, 2, 3, 5], [1, 2, 3, 4, 5]);
```

### Solution to the problem

```javascript
function diffArray(arr1, arr2) {
  let newArr = [];
  for(let i = 0; i < arr1.length; i++){
    if(arr2.indexOf(arr1[i]) !== -1){
      continue;
    }
    newArr.push(arr1[i]);
  }
  for(let j = 0; j < arr2.length;j++){
    if(arr1.indexOf(arr2[j]) !== -1){
      continue;
    }
    newArr.push(arr2[j]);
  }
  return newArr;
}

console.log(diffArray([1,2,3], [3,2,4,5]));
```
