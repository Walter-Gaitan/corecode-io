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
 return words.split(' ').sort(function(a, b) {
    return a.match(/\d/) - b.match(/\d/);
   }).join(' ');
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
function toCamelCase(str){
  first = str.slice(0,1);  
  rest = str.toLowerCase().replace(/[-_]+(.)/g, (m, chr) => chr.toUpperCase());
  return `${first}${rest.slice(1)}`
}
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
### 1. Fold an array
```javascript
function foldArray(array, runs) {   
	if (runs == 0) {
		return array;
	}
	else if (array.length % 2 == 0) {
			let array1 = array.slice(0, array.length / 2)
			let array2 = array.slice(array.length / 2).reverse();
			let sum = array1.map((a, i) => a + array2[i]);
			return foldArray(sum, runs - 1);
		}
		else {
			let array1 = array.slice(0, array.length / 2 + 1)
			let array2 = array.slice(array.length / 2 + 1).reverse();
			array2.push(0);
			let sum = array1.map((a, i) => a + array2[i]);
			return foldArray(sum, runs - 1); 
		}
}
```

### 2. Encrypt this!
```javascript
var encryptThis = function(text) {
  // Implement me! :)
  text = text.split(' ')
  var newText = []
  for (let element of text) {
    toascii = element.charCodeAt(0)
    if (element.length === 1) {
      newText.push(toascii);
    }
    else if (element.length === 2) {
      newText.push(`${toascii}${element.slice(1)}`)
    }
    else {
      newText.push(`${toascii}${element.slice(-1)}${element.slice(2,-1)}${element.slice(1,2)}`)
    } 
  }
  return newText.join(' ');
}
```

### 3.Format a string of names like 'Bart, Lisa & Maggie'. (retired)
```javascript
function list(names){
  //your code here
	var len = names.length;
	if(len == 0) return '';
	var commaNames =  names.slice(0, len-1).map(p=>p.name).join(", ");
	return `${commaNames}${(len>1 ? ' & ' : '')}${names[len-1].name}`
}
```