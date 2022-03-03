# Week 7 Typescript 
---
## 📖 Week challenges (Monday)
1. TicTacToe Using Typescript
```typescript

```

---
## 📖 Week challenges (Tuesday)
1. Generics Using Typescript
```typescript

```
2. Encrypt this!
```typescript

```
3. Make the Deadfish Swim
```typescript
export function parse(data: string): number[] {
  var v = 0, ret = []
  for (var c of data) {
    switch (c) {
      case 'i' : v++;         break;
      case 'd' : v--;         break;
      case 's' : v=v*v;       break;
      case 'o' : ret.push(v); break;
    }
  }
  return ret;
}
```
---
## 📖 Week challenges (Wednesday)
1. More About Generics 
2. Read and follow this
3. Read and follow this
4. Dashatize it
```typescript
export const dashatize = (num: number) => {
 return String(num)
    .replace(/([13579])/g, "-$1-")
    .replace(/--+/g, "-")
    .replace(/(^-|-$)/g, "")
};
```
---
## 📖 Week challenges (Thursday)
1. Type Predicate
2. Count the smiley faces!
```typescript
export function countSmileys(arr: string[]) {
  return arr.filter(v=>v.match(/(:|;)(-|~)?(\)|D)/)).length
}
```
3. Human Readable Time
```typescript

```
4. Base64 Encoding
```typescript

```
5. Complete your 4th Core Challenge, the Scrum Essentials Certification. (In Progress)
