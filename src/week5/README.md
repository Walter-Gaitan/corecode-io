# Typescript - Week 5

## Week goal 🏁
Learn about classes, instances, inheritance and data type with Typescript

---
## Week challenges (Monday) 💻

### 1. Typescript primitives, type aliases and interfaces

<div style="text-align: justify">Here we learn about the different 
types that we encounter such as booleans, numbers and strings. Here is important to know that when you select a type, you can't create a variable with a value that is not congruent with the type. But you can select more than one type (ex: number || string).<br><br>
After that we begin with type aliases which are basically types created by the user as a template so redundancy is avoided. Interfaces are just another way to name object types, it is very similar to aliases with the only difference that the first one cannot be modified and the second one can be extended at any moment.</div>

---
 **NOTE**
The following exercises are written in Typescript, which is similar to Javascript but enhanced. 

---


### 2. Square(n) Sum
```typescript
export function squareSum(numbers: number[]): number {
  let square = numbers.map(function(x){ return x ** 2 });
  let sum = 0;
  for (let i = 0; i < square.length; i++) {
      sum += square[i];
  }
  return sum;
}
```

### 3. Growth of a Population
```typescript
export class G964 {

  public static nbYear = (p0, percent, aug, p) => {
      // your code
      for (var years = 0; p0 < p; years++) {
      p0 += ((p0 * (percent * 0.01)) + aug);
      }
  return years;
  }
}
```

### 4. Mumbling
```typescript
export function accum(s: string): string {
  let chars = s.split('');
  let arr = []
  for (let i = 0; i < chars.length; i++) {
      arr.push(`${chars[i].toUpperCase()}${chars[i].repeat(i).toLowerCase()}`)
  }
  return arr.join('-');
}
```

### 5. A wolf in sheep's clothing
```typescript
export function warnTheSheep(queue: string[]): string {
    if (queue[queue.length -1] === 'wolf') {
        return 'Pls go away and stop eating my sheep';
    } else {
        let index = queue.findIndex( (x) => x == 'wolf' );
        return `Oi! Sheep number ${queue.length - index - 1}! You are about to be eaten by a wolf!`;
    };
}
```

## Week challenges (Tuesday) 💻

### 1. A Rule of Divisibility by 13
```typescript
export function thirt(n: number): number {
    // your code
  const sequence = [1, 10, 9, 12, 3, 4];
  let nums = n.toString().split('').reverse()
  let res = nums.map( (c,i) => parseInt(c)*sequence[i%6]).reduce( (p,c) => p += c );
  return n == res ? res : thirt(res)
}
```

### 2. Playing with digits
```typescript
export class G964 {

    public static digPow = (n: number, p: number) => {
        // your code
        var digits = n.toString().split('');
        var result = 0;
        
        for(var i=0; i<digits.length; i++) {
            result = result + Math.pow(parseInt(digits[i]), p);
            p++;
        }
        var data = result/n;
        if(result % n === 0) {
            return data;
        }
        else {
            return -1;
        }
    }
}
```