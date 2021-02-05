# Intermediate Algorithm Scripting: Seek and Destroy

### 

You will be provided with an initial array (the first argument in the destroyer function), followed by one or more arguments. Remove all elements from the initial array that are of the same value as these arguments.

Note
You have to use the arguments object.

### Given

```javascript
//Use arguments Object
// [arguments object] {
//  0:[1, 2, 3, 1, 2, 3]
//  1: 2,
//  2:3
//}
function destroyer(arr) {
  
}

destroyer([1, 2, 3, 1, 2, 3], 2, 3);

```

### Solution to the problem

```javascript
function destroyer(arr) {
  //.Slice will slice the array from position 1 [2,3]
  const newArray = [...arguments].slice(1);
  const finalArray = [];
  for (let i = 0; i < arr.length; i++) {
    if (newArray.indexOf(arr[i]) == -1) {
      finalArray.push(arr[i]);
    }
  }
 return finalArray;
}
destroyer([1, 2, 3, 1, 2, 3], 2, 3)

console.log(diffArray([1,2,3], [3,2,4,5]));
```
