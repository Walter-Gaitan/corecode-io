# Typescript - Week 5

## Week goal 🏁
Learn about classes, instances, inheritance and data type with Typescript

---
## Week challenges (Monday) 💻

### 1. Typescript primitives, type aliases and interfaces

<div>Here we learn about the different types that we encounter such as booleans, numbers and strings. Here is important to know that when you select a type, you can't create a variable with a value that is not congruent with the type. But you can select more than one type (ex: number || string).

After that we begin with type aliases which are basically types created by the user as a template so redundancy is avoided. Interfaces are just another way to name object types, it is very similar to aliases with the only difference that the first one cannot be modified and the second one can be extended at any moment.</div>

### 2. Square(n) Sum (using Typescript)
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