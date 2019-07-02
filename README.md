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

* https://www.codewars.com/kata/print-a-rectangle-using-asterisks/train/javascript

```javascript
function getRectangleString(width, height) {
  const rn = '\r\n';
  const topBottom = '*'.repeat(width) + rn;
  const center = (width > 1) ? ('*' + ' '.repeat(width - 2) + '*' + rn).repeat(height - 2) : '';
  return height > 1 ? topBottom + center + topBottom : topBottom.repeat(height);
}
```
* https://www.codewars.com/kata/string-average/javascript

```javascript

function averageString(str) {
  let numStr = ['zero', 'one', 'two', 'three', 'four', 'five', 'six', 'seven', 'eight', 'nine'];
  let sum = 0;
  let floor = 0;
  let f;
  let arrStr = str.split(' ');
  for (let i = 0; i < arrStr.length; i++) {
    f = false;
    for (let q = 0; q < numStr.length; q++) {
      if (arrStr[i] === numStr[q]) {
        sum += q;
        f = true;
      }
    }
    if (!f) return 'n/a';
  }
  floor = Math.floor(sum / arrStr.length);
  return numStr[floor];
}
```

* https://www.codewars.com/kata/5264d2b162488dc400000001

```javascript

function spinWords(str) {
  let arrStr = str.split(' ');

  for (let i = 0; i < arrStr.length; i++) {
    if (arrStr[i].length >= 5) {
      arrStr[i] = arrStr[i].split('').reverse().join('');
    }
  }
  return arrStr.join(' ');
}
```
* https://www.codewars.com/kata/541c8630095125aba6000c00

```javascript

function digital_root(n) {
  let num = 0;
  let nStr = n.toString();
  let digits = [];

  if (n < 9) {
    return num = n;
  } else if (n > 9) {
    for (let i = 0; i < nStr.length; i++) {
      digits.push(nStr[i]);
    }
    for (let i = 0; i < digits.length; i++) {
      num += Number(digits[i]);
    }
  }
  if (num > 9) {
    n = num;
   return digital_root(n)
   }
  return num;
}
```
* https://www.codewars.com/kata/56dec885c54a926dcd001095

```javascript
function opposite(number) {
return number > 0 ? Number(`-${number}`) : number *= -1;
}
```

