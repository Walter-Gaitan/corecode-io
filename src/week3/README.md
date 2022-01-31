# Javascript - Week 3

## Week goal 🏁
Learn about Javascript behaviour

## Week challenges (Monday) 💻

### 1. Who likes it? 

```javascript
  function likes(names) {
  // TODO
  if (names.length > 3) {
    return (`${names[0]}, ${names[1]} and ${names.length - 2} others like this` );
  }
  else if (names.length > 2) {
    return (`${names[0]}, ${names[1]} and ${names[2]} like this`);
  }
  else if (names.length > 1) {
    return (`${names[0]} and ${names[1]} like this`);
  }
  else if (names.length > 0) {
    return (`${names[0]} likes this`);
  }
  else {
    return 'no one likes this'
  }
}
```
### 2. Bit Counting

```javascript
var countBits = function(n) {
  // Program Me
  n = n.toString(2).split('');
  numarray = n.map(Number);
  return numarray.reduce((a, b) => a + b, 0)
};
```
### 3. Decode the Morse code

```javascript
decodeMorse = function( morseCode ) {
    return morseCode
             .split("   ")
             .map(word => word
                           .split(" ")
                           .map(character => MORSE_CODE[character])
                           .join('')
              )
              .join(' ')
              .trim()
}
```

## Week challenges (Tuesday) 💻

### 1. Your order, please

```javascript
function order(words){
  // ...
}
```
### 2. Counting Duplicates
```javascript
function duplicateCount(text){
  
  var count = new Set();
  var letters = new Set(); 
  
  for(var i of text.toLowerCase()) {

    if (letters.has(i)) {
      count.add(i);
    }
    else {
      letters.add(i);
    }
  }
  return count.size;
}
```
### 3. Simple Pig Latin
```javascript
function pigIt(str){
  //Code here
  str = str.split(' ');
  var newstr = []
  const symbols = /[!@#$%^&*()_+\-=\[\]{};':"\\|,.<>\/?]+/;
  
  for (var i = 0; i < str.length; i++) {
    let letter = str[i].slice(0, 1)
    
    if (symbols.test(str[i])) {
      newstr.push(str[i]);
    }
    else {
      newstr.push(str[i].slice(1) + letter + 'ay');
    }
  } 
  return newstr.join(' ');
}
```

## Week challenges (Wednesday) 💻

### 1. Valid Parentheses
```javascript
function validParentheses(parens) {
  // your code here ..
  let stack = [];
  for (let i = 0; i < parens.length; i++) {
    let char = parens[i];
    if (char == '(') {
      stack.push(char);
      continue;
    }
    if (char == ')' && stack[0] == '(') {
        stack.pop();
      }
    else {
      return false;
      break;
    }
  }
    return (stack.length == 0);
}
```
### 2. Convert string to camel case
```javascript

```
### 3. Unique In Order
```javascript
var uniqueInOrder=function(iterable){
  //your code here - remember iterable can be a string or an array
  var uniques = []
  for (let i = 0; i < iterable.length; i++) {
    if (iterable[i] === iterable[i+1]) {
      continue;
    }
    else {
      uniques.push(iterable[i])
    }
  }
  return uniques;
}
```

## Week challenges (Thursday) 💻
### 1. 
```javascript
