
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
