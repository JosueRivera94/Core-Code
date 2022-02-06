# Week 2 Javascript
---
## Week challenges (Monday)

Q1. Follow the github course. Done
Q2. Watch this video. Done
Q3. Read this. Done
Q3. Create an account in Codewars. Done

## Week challenges (Tuesday)

Q0. Watch this video. Done
Q1. https://www.codewars.com/kata/50654ddff44f800200000004 (Multiply)
```javascript
	function multiply(a, b){
	  return a*b
	}
```
Q2. https://www.codewars.com/kata/572b6b2772a38bc1e700007a (ASCII Total)
```javascript
	function uniTotal (string) {
	 let suma=0;
	  for(var i=0; i<string.length;i++){
	    suma=suma+string.charCodeAt(i);
	  }
	  return suma;
	}
```
	
Q3. https://www.codewars.com/kata/55ad04714f0b468e8200001c  (get character from ASCII Value)
```javascript
	function getChar(c){
	  let char = String.fromCharCode(c);
	   return char;
	}
```

Q4. https://www.codewars.com/kata/551f37452ff852b7bd000139  (Binary Addition)
```javascript
	function addBinary(a,b){
	  let add = a+b;
	  let cB= add.toString(2);
	  return cB;
	}
	console.log(addBinary(5,3))
```
Q5. https://www.codewars.com/kata/5ad0d8356165e63c140014d4 (Student's Final Grade)

## Week challenges (Wednesday)
1. https://www.codewars.com/kata/57e92e91b63b6cbac20001e5
```javascript
function dutyFree(normPrice, discount, hol){
  let b=0;
  b=parseInt(hol / (discount / 100.0 * normPrice)) ;
    return b;
}
```
2. https://www.codewars.com/kata/5b853229cfde412a470000d0
```javascript
function twiceAsOld(dadYearsOld, sonYearsOld) {
  let a=0;
  a=(dadYearsOld - 2 * sonYearsOld);
  return Math.abs(a);
}
```

3. https://www.codewars.com/kata/5f77d62851f6bc0033616bd8
```javascript
function validSpacing(s) {

 const reg = /(^\s|\s$|\s{2,})/;
  return !(reg.test(s));
}
```

4. https://www.codewars.com/kata/57eae65a4321032ce000002d
```javascript
function fakeBin(x){
 return x.split('').map((num) => num > 4 ? 1 : 0).join('');
}
```

## Week challenges (Thursday)
1. https://www.codewars.com/kata/57faece99610ced690000165
```javascript
function remove (string) { 
let palabra = string;

  while (palabra[palabra.length - 1] === "!") {
    palabra = palabra.slice(0, -1);
  }

  return palabra;
}
```

2. https://www.codewars.com/kata/5547929140907378f9000039
```javascript
function shortcut (string) {
  const vowels = /[aeiou]/g;
  return string.replace(vowels, "");
}
```
3. https://www.codewars.com/kata/5672a98bdbdd995fad00000f
```javascript
const rps = (p1, p2) => {
  if (p1 === p2) {
    return `Draw!`;
  }
  if (p1 === 'rock' && p2 === 'scissors') {
    return `player 1 won!`;
  } else if (p1 === 'scissors' && p2 === 'paper') {
    return `player 1 won!`;
  } else if (p1 === 'paper' && p2 === 'rock') {
    return `player 1 won!`;
  } else if (p1 === 'scissors' && p2 === 'rock') {
    return `player 2 won!`; 
  }else if (p1 === 'paper' && p2 === 'scissors') {
    return `player 2 won!`;
  }else if (p1 === 'rock' && p2 === 'paper') {
    return `player 2 won!`;
  }
};
```

4. https://www.codewars.com/kata/55bf01e5a717a0d57e0000ec
```javascript
function persistence(num) {
  if (typeof num !== 'number') {
    return;
  }
  let count = 0
  let mult = num
  while (true) {
    if (mult < 10) {
      return count;
    }
    mult = [...String(mult)].reduce((a, b) => a * b, 1);
    count++
  }
}
```

5. Complete your 1st Core Challenge. (DONE)
