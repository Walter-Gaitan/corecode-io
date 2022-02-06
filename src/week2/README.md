# Javascript - Week 2

## Week goal ?èÅ

<div style="text-align: justify"> In the second week we choose Javascript to be our predilect programming language and from now on we are working on excercises based on it.</div>

 ---

## Week challenges (Tuesday) ?íª

### 1. Multiply

```javascript
function multiply(a, b){
  return a * b
}
```

### 2. ASCII Total

```javascript
function uniTotal(str) {
  var count = 0;
  for (var i = 0; i < str.length; i++) {
    count += str.charCodeAt(i);
  }
  return count;
}
```

### 3. get character from ASCII Value

```javascript
function getChar(c){
return c = String.fromCharCode(c);
}
```

### 4. Binary Addition

```javascript
function addBinary(a,b) {
  sum = a + b
  return sum.toString(2);
}
```

### 5. Student's Final Grade

```javascript
function finalGrade (exam, projects) {
  if (exam > 90 || projects > 10){
    return 100;
  }
  else if (exam > 75 && projects >= 5){
    return 90;
  }
  else if (exam > 50 && projects >= 2){
    return 75;
  }
  else {
    return 0
  }
}
```

---

## Week challenges (Wednesday) ?íª

### 1. Holiday VIII - Duty Free

```javascript
function dutyFree(normPrice, discount, hol){
  cutPrice = normPrice * discount / 100
  total = hol / cutPrice
  return Math.floor(total)
}
```

### 2. Twice as old

```javascript
function twiceAsOld(dadYearsOld, sonYearsOld) {
  twice = sonYearsOld * 2
  if (dadYearsOld > twice){
    return dadYearsOld - twice;
  }
  else {
    return twice - dadYearsOld;
  }
}
```

### 3. Valid Spacing

```javascript
function validSpacing(s) {
  if (s[0] == ' ' || s.slice(-1) == ' ' || s.includes('  ')) {
    return false;
  }
  else {
    return true;
  }
}
```

### 4. Fake Binary

```javascript
function fakeBin(x){
  x = x.toString().split('')
  const bin = []

  for (var i in x){
    if (x[i] < 5){
      bin.push(0);
    }
    else {
      bin.push(1);
    }
  }
  return bin.join('');
}
```

---

## Week challenges (Thursday) ?íª

### 1. Remove all exclamation marks from the end of sentence

```javascript
function remove (string) {  
  while (true) {
  if (string.slice(-1) == '!') {
    string = string.slice(0, -1);
  }
  else {
    break;
  }}
  return string
}
```

### 2. Vowel remover

```javascript
function shortcut (string) {
  return   string = string.replace(/[aeiou]/ig, '');
}
```

### 3. Rock Paper Scissors

```javascript
const rps = (p1, p2) => {
if (p1 == 'scissors' && p2 == 'paper' || p1 == 'rock' && p2 == 'scissors' || p1 == 'paper' && p2 == 'rock'){
  return 'Player 1 won!'
}
  else if (p1 == 'scissors' && p2 == 'rock' || p1 == 'paper' && p2 == 'scissors' || p1 == 'rock' && p2 == 'paper'){
    return 'Player 2 won!'
  }
  else if(p1 == p2){
    return 'Draw!'
  }
};
```

### 4. Persistent Bugger

```javascript
function persistence(num) {
  var count = 0;
  num = num.toString()
  while (num.length > 1) {
    count++;
    num = num.toString().split('').map(Number).reduce((a, b) => a * b).toString();
    }
  return count;
  } 
```

---

5. ## ?éØ Mission statement
   
   <div style="text-align: justify"> I am Walter G, currently I have a role as an IT Support Specialist. My learning objectives are focused on the emerging technology of cloud computing with companies like Google Cloud and Microsoft Azure, and I am planning to use my knowledge in the DevOps area one day. Also, I have some knowledge in web development and Python, focused on data science. </div>
