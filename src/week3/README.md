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
             .split("   ") // get word code 3 spaces apart
             .map(word => word
                           .split(" ") // get character code 1 spaces apart
                           .map(character => MORSE_CODE[character]) // decode Morse code character
                           .join('')
              )
              .join(' ') // add spaces between words 
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

## Week challenges (Wednesday) 💻

### 1. Valid Parentheses
```javascript
function validParentheses(parens) {
  // your code here ..
  if (parens.length % 2 != 0) {
    return false;
  }
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
    return (stack.length == 0);
  }
}