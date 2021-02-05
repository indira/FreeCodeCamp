# Sum All Numbers in a RangePassed

### 

We'll pass you an array of two numbers. Return the sum of those two numbers plus the sum of all the numbers between them. The lowest number will not always come first.

For example, sumAll([4,1]) should return 10 because sum of all the numbers between 1 and 4 (both inclusive) is 10

### Given

```javascript
function sumAll(arr) {
  return 1;
}

sumAll([1, 4]);
```

### Solution to the problem

```javascript
function sumAll(arr) {
  const min = Math.min(...arr);
  const max = Math.max(...arr);
  let sum = 0;
  for(let i = min; i <= max; i++){
     sum += i;
  }
  return sum;
}

console.log(sumAll([5, 10]));
```
