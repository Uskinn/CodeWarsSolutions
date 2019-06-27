Hello

--------------

* https://www.codewars.com/kata/5a2be17aee1aaefe2a000151

```javascript

function arrayPlusArray(arr1, arr2) {
  let sum1 = 0;
  let sum2 = 0;
  for (let i = 0; i < arr1.length; i++) {
    sum1 += arr1[i];
  }
  for (let j = 0; j < arr2.length; j++) {
    sum2 += arr2[j];
  }
  return sum1 + sum2;
}
```

* https://www.codewars.com/kata/pick-a-set-of-first-elements/train/javascript

```javascript
function first(arr, n = 1) {
  let returnArr = [];
  if (n > arr.length) {
    return arr;
  }
  for (let i = 0; i < n; i++) {
    returnArr.push(arr[i]);
  }
  return returnArr;
```

* https://www.codewars.com/kata/57073869924f34185100036d

```javascript
function randomCase(x) {
  return x.split('').map(function(element) {
    return Math.random() > 0.5 ? element.toUpperCase() : element.toLowerCase();
  }).join('');
}
```