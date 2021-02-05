#Basic Algorithm Scripting: Return Largest Numbers in ArraysPassed
###Return an array consisting of the largest number from each provided sub-array. For simplicity, the provided array will contain exactly 4 sub-arrays.

Remember, you can iterate through an array with a simple for loop, and access each member with array syntax arr[i].
### 
```Javascript Given
function largestOfFour(arr) {
  let array = [];
  return array;
 }
```
### Solution to the problem
```JavaScript
function largestOfFour(arr) {
	//Define an empty array ('array') to store the result
	let array = [];
	for(let i = 0; i < arr.length; i++){
	let maxNum =0;
		for(let j = 0; j < arr[i].length;j++){
			  if(maxNum < arr[i][j]){
				maxNum = arr[i][j];
			  }
		}
		array.push(maxNum);
	}
	return array;
}
console.log(largestOfFour([[17, 23, 25, 12], [25, 7, 34, 48], [4, -10, 18, 21], [72, 3, 17, 10]]));

```