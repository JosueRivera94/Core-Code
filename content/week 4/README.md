# Week 4 npm,npx & Typescript 
---
## 📖 Week challenges (Monday)
1. Check this video: 
  Regular Expressions (RegEx) in 100 Seconds (DONE).
2. Follow this video:
  Regular Expressions (Regex) in JavaScript - tutorial (DONE).
3. Follow this guide:
  JavaScript RegEx Exercises 01 (DONE).
4. Check this video:
  JavaScript Promise in 100 Seconds (DONE).
5. Follow this video:
  JavaScript Promises In 10 Minutes (DONE).
6. Check this video:
  ¿Cómo funcionan las Promises y Async/Await en JavaScript? (DONE).

---
## 📖 Week challenges (Tuesday)
1. This link is nice to have and read:
  The TypeScript Handbook (DONE).
2. Typescript object type:
3. Read this:
  Types vs. interfaces in TypeScript (DONE).
4. Typescript union types: 
5. Typescript in operator:
6. Find the odd int:

```javascript
function findOdd(A) {
let count = 0;
  let arr = A.sort((a, b) => a - b);
  for (let i = 0; i < arr.length; i++) {
    for (let j = 0; j < arr.length; j++) {
      if (arr[i] == arr[j]) {
        count++;
      }
    }
    if (count % 2 !== 0) {
      return arr[i];
    }
  }
}
```

7. Stop gninnipS My sdroW!:
```javascript
function spinWords(string){
 const sentenceArray = string.split(' ');
  let result = '';
  sentenceArray.map((str, i) => {
    if (str.length >= 5){
      sentenceArray[i] = str.split('').reverse().join('');
    } else {
      sentenceArray[i] = str;
    }
  result = sentenceArray.join(' ');
  });
return result;
}

```
  
---
## 📖 Week challenges (Wednesday)
1. Array.diff
```javascript
function arrayDiff(a, b) {
    return a.filter(val => !b.includes(val));
   }
```

2. Create Phone Number
```javascript
 function createPhoneNumber(numbers){
    let mask = '(xxx) xxx-xxxx';
 
     numbers.forEach(item => {
         mask = mask.replace('x', item);
     });
 
     return mask;
   }
```
3. Watch this:  
  Fundamental Concepts of Object Oriented Programming (DONE):
4. Watch this:
  FP vs OOP | For Dummies (DONE).
5. Read this:
  OOP: Everything you need to know about Object Oriented Programming (DONE).
6. Read this:
  TypeScript — OOP’s Concepts (DONE).
7. Read this:
  TypeScript — Object Oriented Programming (DONE).

---
## 📖 Week challenges (Thursday)
1. Detect Pangram
```javascript
function isPangram(string){
string = string.toLowerCase();
  return "abcdefghijklmnopqrstuvwxyz"
    .split("").every(function(x){
      return string.indexOf(x) !== -1;
  });
}
```

2. Find the missing letter
```javascript
function findMissingLetter(array)
{
return String.fromCharCode(array.find((c,i)=>array[i+1].charCodeAt()-c.charCodeAt()!==1).charCodeAt()+1)
}
```

3. Find the unique number
```javascript
function findUniq(arr) {
return +arr.filter( (value) => { return arr.indexOf(value) == arr.lastIndexOf(value) } );
}
```

4. Reverse or rotate?
```javascript
const G964 = (arr, slice) => {
    let arrNum = [];
    let reverseCondition = [];
    let cont = 0;
    if (slice <= 0 || arr == '' || slice > arr.length)
        return '';
    if (slice == arr.length)
        return arr;
    for (let i = 0; i < arr.length; i += slice) {
        let chunck = arr.split('').map((x) => parseInt(x)).splice(i, i + slice);
        arrNum.push(chunck);
    }
    reverseCondition = arrNum.map((x) => {
        return x.reduce((acc, el) => {
            acc += el * el * el;
            return acc;
        }, 0) % 2 === 0;
    });
    for (let i = 0; i < reverseCondition.length; i++) {
        if (reverseCondition[i] == true)
            arrNum[i] = arrNum[i].reverse();
        else {
            arrNum[i].push(arrNum[i][0]);
            arrNum[i] = arrNum[i].slice(1);
        }
    }
    arrNum = arrNum.map((x) => {
        return x.join('').toString();
    });
    return arrNum.join('');
};
console.log(G964("330479108928157", 5));
}
```

5. What's Your Poison?
```javascript
function find(rats) {
  return rats.reduce((a,b)=>a+Math.pow(2,b),0)
}
```
6. Complete your 3rd Core Challenge. GitHub Boost Guide! (DONE)

