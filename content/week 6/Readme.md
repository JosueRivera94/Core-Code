# Week 6 Typescript 
---
## 📖 Week challenges (Monday)
1. Read this (DONE). Sumary:<br>
Input class, this class can be use to get different inputs from the user,

2.Menu Using Typescript
```typescript

```

---
## 📖 Week challenges (Tuesday)
1. Movies Using Typescript.
```typescript

```
2. Readme. in a md file, you are going to create a OOP glossary

3. Interfaces. Implement interfaces in TypeScript
---
## 📖 Week challenges (Wednesday)
1. Build Tower Using Typescript
```typescript
export const towerBuilder = (nFloors: number): string[] => {
 return [...Array(nFloors)].map((_,i)=>" ".repeat(nFloors-1-i)+"*".repeat(i*2+1)+" ".repeat(nFloors-1-i))
}
```
2. Highest Scoring Word Using Typescript
```typescript
export const high = (str: string): string =>{
  let as = str.split(' ').map(str=>[...str].reduce((a,b)=>a+b.charCodeAt(0)-96,0));
  return str.split(' ')[as.indexOf(Math.max(...as))];
}
```
3. Equal Sides Of An Array Using Typescript (x)
```typescript
export function findEvenIndex(arr: number[]): number
{
  for(var i=1; i<arr.length-1; i++) {
    if(arr.slice(0, i).reduce((a, b) =>  a+b) === arr.slice(i+1).reduce((a, b) =>  a+b)) {
      return i;
    }
  }
  return -1;
}
```
4. Meeting Using Typescript
```typescript
export function meeting(s: string): string {
  return s.replace(/;/gi,' ').split(' ').map(v=>v.split(':').reverse().join(', ').toUpperCase()).sort()
   .map(v=>'('+v+')').join('')
}
```
5. Street Fighter 2 - Character Selection Using Typescript
```typescript
export function streetFighterSelection(fighters: Array<string[]>, position: number[], moves: string[]) {
  let arr=[];
  let y=position[0];
  let x=position[1]
  for (let i=0;i<moves.length;i++){
  if (moves[i]==='left'){x--;if(x<0){x=5}arr.push(fighters[y][x])}
  if (moves[i]==='right'){x++;if(x>5){x=0}arr.push(fighters[y][x])}
  if (moves[i]==='up'){y++;if(y>0){y=0}arr.push(fighters[y][x])}
  if (moves[i]==='down'){y--;if(y<1){y=1}arr.push(fighters[y][x])}} 
  return arr;
}
```
---
## 📖 Week challenges (Thursday)
1. Watch Object Oriented Programming - The Four Pillars of OOP (DONE)
2. Watch Abstract Classes vs Interfaces (DONE)
3. Read Abstract Classes (DONE)
