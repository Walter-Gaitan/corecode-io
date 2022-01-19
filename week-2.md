## Week challenges (Tuesday) 💻
1. 
```javascript
function multiply(a, b){
  return a * b
}
```
2. 
```javascript
function uniTotal(str) {
  var count = 0;
  for (var i = 0; i < str.length; i++) {
    count += str.charCodeAt(i);
  }
  return count;
}
```
3. 
```javascript
function getChar(c){
return c = String.fromCharCode(c);
}
```
4. 
```javascript
function addBinary(a,b) {
  sum = a + b
  return sum.toString(2);
}
```
5. 
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
## Week challenges (Wednesday) 💻
1. 
```javascript
function dutyFree(normPrice, discount, hol){
  cutPrice = normPrice * discount / 100
  total = hol / cutPrice
  return Math.floor(total)
}
```
2. 
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
3. 
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
4. 
```javascript
