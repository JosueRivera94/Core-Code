# Week 5 Typescript 
---
## 📖 Week challenges (Monday)
1. Read this from The primitives: string, number and boolean to Differences Between Type Aliases and Interfaces section (DONE) <br>
  summary: Type aliases and interfaces are very similar, and in many cases you can choose between them freely. <br>
  Almost all features of an interface are available in type, the key distinction is that a type cannot be re-opened to add new properties vs an interface which is always             extendable. <br>
  
2. Square(n) Sum Using Typescript
```typescript
  export function squareSum(numbers: number[]): number {
   var total = 0;

  for(var i = 0; i < numbers.length; i++) {
    total += numbers[i] * numbers[i]; 
    }
  return total;
}
```

3. Growth of a Population Using Typescript
```typescript
  export class G964 {

    public static nbYear = (p0, percent, aug, p) => {
       var i = 0;
        while (true) {
          if (p0 >= p) {return i;}
            p0 = p0 * (1 + percent/100) + aug; i++;
        }
        }
}
```


4. Mumbling Using Typescript
```typescript
export function accum(s: string): string {
  const result = []
  const lowerStr = s.toLowerCase()

  for(let i = 0; i < lowerStr.length; i++) {
    let str = lowerStr[i].toUpperCase()
    for(let j = 0; j < i; j++) {
      str += lowerStr[i]
    }
    result.push(str)
  }

  return result.join("-")
}

```
5. A wolf in sheep's clothing Using Typescript
```typescript
export function warnTheSheep(queue: string[]): string {
   if (queue[queue.length -1] === 'wolf') {
    return 'Pls go away and stop eating my sheep';
    } else {
     let index = queue.findIndex( (x) => x == 'wolf' );
     return `Oi! Sheep number ${queue.length - index - 1}! You are about to be eaten by a wolf!`;
    }
}

```


---
## 📖 Week challenges (Tuesday)
1. A Rule of Divisibility by 13 Using Typescript (X)
```typescript
export function thirt(n: number): number {
  const dict=[1, 10, 9, 12, 3, 4]
   let sum=n;
   while(1){
       let temp=sum
       sum=sum.toString().split``.reverse().join``.split``.map((v,i)=>{
         v=v*dict[i%6]
         return v
       }).reduce((a,b)=>a+b,0)
       if (sum===temp){break}
     }
   return sum
}

```

2. Playing with digits Using Typescript
```typescript
export class G964 {

    public static digPow = (n: number, p: number) => {
       let arr=n.toString().split('').map(Number).reduce((acc,cur,i,arr)=>acc+(Math.pow(arr[i],p+i)),0)/n
       return (''+arr).includes('.')?-1:arr
    }
}

```

3. Valid Braces Using Typescript
```typescript
export function validBraces(braces: string): boolean {
  while(/\(\)|\[\]|\{\}/g.test(braces)){braces = braces.replace(/\(\)|\[\]|\{\}/g,"")}
  return !braces.length;
}

```
4. Tic-Tac-Toe Using Javascript
```typescript


```

5. Tic-Tac-Toe-like table Generator Using Javascript
```typescript


```
---
## 📖 Week challenges (Wednesday)
1. Duplicate Encoder Using Typescript
```typescript
export function duplicateEncode(word: string){
    return word
    .toLowerCase()
    .split('')
    .map( function (v, i, arr) {
      return arr.indexOf(v) == arr.lastIndexOf(v) ? '(' : ')'
    })
    .join('');
}

```
2. Find the odd int Using Typescript
```typescript
export const findOdd = (xs: number[]): number => {
  for(let i = 0; i < xs.length; i++){
    const count = xs.filter(value => value === xs[i]).length;
    if(count % 2 == 1){
      return xs[i];
    }
  }
  return -1;
};

```
3. Which are in? Using Typescript
```typescript
export class G964 {
  public static inArray(a1: string[], a2: string[]): string[] {
   let arr = a2.join(" ")
  return a1.filter(item => arr.search(item) !== -1 && item !== undefined ).sort()
  }
}

```
4. Sums of Parts Using Typescript
```typescript
export function partsSums(ls: number[]): number[] {
  let arr = [0];
  ls.reverse().forEach(v => arr.push(arr[arr.length-1] + v));
  return arr.reverse();
}

```
5.  Consecutive strings Using Typescript
```typescript
export function longestConsec(strarr: string[], k: number): string {
   var longest = "";
    for(var i=0;k>0 && i<=strarr.length-k;i++){
      var tempStr = strarr.slice(i,i+k).join("");
      if(tempStr.length > longest.length){
        longest = tempStr;
      }
    }
    return longest;
}

```
---
## 📖 Week challenges (Thursday)
1. Tile Using Typescript
```typescript


```
2. Time Using Typescript
```typescript


```
3. Rational Using Typescript
```typescript


```


4.  Complete your 4th Core Challenge (In Progess)
