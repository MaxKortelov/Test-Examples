# Test-Examples
This repository is intended for study purposes and contains only selected tasks and examples

```let n = '',
		arr = ["0", "1"],
    arr1 = [],
    num = 6;

function sortOut(arr, num) {
	num === 1 ?
  	 ( arr.flatMap(el => {n += el; arr1.push(n); n = n.slice(0, -1)}) ) :
   ( arr.flatMap(el => {n += el; sortOut(arr, num - 1); n = n.slice(0, -1)}) );
}

sortOut(arr, num);
console.log(arr1);```
