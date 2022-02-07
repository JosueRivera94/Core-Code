# Week 3 Javascript
---
## 📖 Week challenges (Monday)
1. https://www.codewars.com/kata/5266876b8f4bf2da9b000362
```javascript
function likes(names) {
    if (names.length == 0) {
      return "no one likes this";
    } 
    else if (names.length == 1) {
      return names[0] + " likes this";  
    } 
    else if (names.length == 2) {
      return names[0] + " and " + names[1] + " like this";
    } 
    else if (names.length == 3) {
      return names[0] + ", " + names[1] + " and " + names[2] + " like this";
    } 
    else {
      return names[0] + ", " + names[1] + " and " + (names.length - 2) + " others like this";
    }
  }
  ```

2. https://www.codewars.com/kata/526571aae218b8ee490006f4
```javascript
var countBits = function(n) {
    const base = (n).toString(2).split('');
    
    const result = base.reduce((sum, num) => sum + Number(num), 0);
    
    return result;

 };
  ```
  
3. https://www.codewars.com/kata/54b724efac3d5402db00065e
```javascript
decodeMorse = function(morseCode){
    morseCode = morseCode.trim();
  let refinedData = morseCode.split('   ');
  let result = [];
  
  for (let i = 0; i < refinedData.length; i++) {
    let temp = refinedData[i].split(' ');
    for (let j = 0; j < temp.length; j++) {
      if (MORSE_CODE[temp[j]]) {
        result.push(MORSE_CODE[temp[j]]);
      }
    }
    
    if (i !== refinedData.length - 1) {
    result.push(' ');
    }
  }
  return result.join('');
}
  ```
  
---
## 📖 Week challenges (Tuesday)
1. https://www.codewars.com/kata/55c45be3b2079eccff00010f
```javascript
function order(words){
    return words.split(' ').sort(function(a,b){
        return a.match(/\d/) - b.match(/\d/);
      }).join(' ');
}
  ```

2. https://www.codewars.com/kata/54bf1c2cd5b56cc47f0007a1
```javascript
function duplicateCount(text){
    let result = 0,
      soltingObject = {};
  text.toLowerCase().split('').map(str => {
      if (!soltingObject.hasOwnProperty(str)) {
        soltingObject[str] = 0;
      } else {
        if (soltingObject[str] === 0) {
          result += 1;
        }
        soltingObject[str] = soltingObject[str] + 1;
      }
  });
  return result;
  }
 ```

3. https://www.codewars.com/kata/520b9d2ad5c005041100000f
```javascript
 function pigIt(str){
    let strArr = str.split(' ');
  let pigLatin = [];

  for(let word of strArr){
    if((/([a-zA-Z])/).test(word)){
      pigLatin.push(word.substring(1) + word[0] + "ay");
    }else{
      pigLatin.push(word);
    }
  }
  return pigLatin.join(" ");
}
 ```

---
## 📖 Week challenges (Wednesday)
1. https://www.codewars.com/kata/52774a314c2333f0a7000688
```javascript
function validParentheses(parens) {
var indent = 0;
  
  for (var i = 0 ; i < parens.length && indent >= 0; i++) {
    indent += (parens[i] == '(') ? 1 : -1;    
  }
  
  return (indent == 0);
}
 ```

2. https://www.codewars.com/kata/517abf86da9663f1d2000003
```javascript
function toCamelCase(str){
str = str.split('');
  return str.map(function(el, i){
    if(el == '-' || el == '_'){
      el = str[i+1].toUpperCase();
      str.splice(i+1, 1);
    }
    return el;
  }).join('');
}
 ```

3. https://www.codewars.com/kata/54e6533c92449cc251001667
```javascript
var uniqueInOrder=function(iterable){
 if(iterable.length == 0) return [];
  var stage= [iterable[0]];
  if(typeof iterable === 'string'){
    iterable = iterable.split('');
  }  
  iterable.reduce(function(pre,cur){
    if(pre != cur){
      stage.push(cur)
    }
    return cur;
  });
  return stage
}
 ```

---
## 📖 Week challenges (Thursday)
1. https://www.codewars.com/kata/57ea70aa5500adfe8a000110
```javascript
function foldArray(array, runs)
{
  const r = [], c = array.slice();
  while (c.length) r.push(c.pop() + (c.shift() || 0));
  return runs - 1 ? foldArray(r, runs - 1) : r;
}
 ```

2.https://www.codewars.com/kata/5848565e273af816fb000449
```javascript
var encryptThis = function(text) {
  if(text === '') {return '';
    }else {
        let s = text.split(' ');
        let x = s.map(element => {
            let a = element.split('');
            a[0] = element.charCodeAt(0);
            [a[1], a[a.length - 1]] = [a[a.length - 1], a[1]];
            return a.join('');});
      return x.join(' ');
    }
}
 ```

3.https://www.codewars.com/kata/53368a47e38700bd8300030d
```javascript
function list(names){
  if(names.map(v=>v.name).length>1) return names.map(v=>v.name).slice(0,-1).join(', ')+' & '+names.map(v=>v.name).slice(-1)
  return names.map(v=>v.name).slice(-1)+''
}
 ```

4. Complete your 2nd Core Challenge. 
