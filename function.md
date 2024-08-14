# Functions in JavaScript

### `main()`

```javascript
function main() {
  console.log('Hello, world!');
}

main();
```

### `add()` and `return`

```javascript
function add() {
  return 1 + 2;
}

let result = add();
console.log(result);
```

### Function with parameters

```javascript
function add(a, b) {
  return a + b;
}

let result = add(1, 2);
console.log(result);

let result2 = add(2, 2);
console.log(result2);

let result3 = add(3, 2);
console.log(result3);

let result4 = add(4, 2);
console.log(result4);
```

### Function with conditional statements and loops

```javascript
function table(n) {
    if (n === 1 || n === 0) {
        console.log(`Table of ${n} is not possible`);
    } else {
        for (let i = 1; i <= 10; i++) {
            console.log(`${n} x ${i} = ${n * i}`);
        }
    }
}

table(1);
```