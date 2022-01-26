## Week goal 🏁
Learn about Javascript behaviour

## Week challenges (Monday) 💻
1. 
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
2. 
```javascript
var countBits = function(n) {
  // Program Me
  n = n.toString(2).split('');
  numarray = n.map(Number);
  return numarray.reduce((a, b) => a + b, 0)
};
```
3. 
```javascript

```

## Week challenges (Tuesday) 💻

### 1. Your order, please

```javascript
function order(words){
  // ...
}