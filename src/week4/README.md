# npm,npx & Typescript - Week 4

**NOTE**

Since the challenges are watching videos and learning about npm, npx and Typescript I decided just to post a review of what I learn.

---

## Week challenges (Monday) 💻

### 1. RegExp

 So the first thing to talk about is RegEx, basically is a special syntax that you can use across multiple languages to find specific patterns in a string. You can create a patterns that suits you using numbers, symbols, letters and the combinations of them to add, remove or replace parts in the string. It may seem very complicated but you can use tools to help you out creating your RegEx format like [RegExr](https://regexr.com/).

### 2. Promises

As it sounds, promises are statements that you compromise to accomplish in the future, so the code runs based on this from happening at some moment, which makes webpages and applications run faster while the action has not been executed yet. If you don't keep your promise there is also the option to execute something different to show that things didn't happen as expected. 

## Week challenges (Tuesday) 💻

### 2. TypeScript object type

```typescript
export type User = {
    name: string;
    age: number;
    occupation: string;
};

export const users: User[] = [
    {
        name: 'Max Mustermann',
        age: 25,
        occupation: 'Chimney sweep'
    },
    {
        name: 'Kate Müller',
        age: 23,
        occupation: 'Astronaut'
    }
];

export function logPerson(user: User) {
    console.log(` - ${user.name}, ${user.age}`);
}
```

### 3. Types vs. interfaces in TypeScript

### 6. Find the odd Int

```javascript
function findOdd(A) {
  //happy coding!
  const counts = {};
  A.forEach((x) => {counts[x] = (counts[x] || 0) + 1});
  for (const key in counts) {
    if (counts.hasOwnProperty(key) && counts[key] % 2 != 0) {
        return parseInt(key)
    }
  }
}
```

## Week challenges (Wednesday) 💻

### 1. Array.diff

```javascript
function arrayDiff(a, b) {
   const bSet = new Set(b);
   const newArr = a.filter((name) => {return !bSet.has(name)});
   return newArr;
}
```

### 2. Create Phone Number

```javascript
function createPhoneNumber(numbers){
  const countryCode = numbers.slice(0,3).join('');
  const first = numbers.slice(3,6).join('');
  const last = numbers.slice(6).join('');
  return `(${countryCode}) ${first}-${last}`
}
```

## Week challenges (Thursday) 💻

### 1. Detect Pangram

```javascript
function isPangram(string){
  return new Set(string.toLowerCase().match(/[a-z]/g)).size === 26;
}
```

### 2.