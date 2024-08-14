# Arrays in JavaScript

In JavaScript, an array is a data structure that can hold multiple values, of various data types, under a single variable name. Arrays are zero-indexed, meaning the first element is at index `0`, the second at index `1`, and so on.


You can create an array in JavaScript using:
- **Array Literal Syntax:**
  ```javascript
  let fruits = ["Apple", "Banana", "Mango"];
  ```
- **Array Constructor:**
  ```javascript
  let fruits = new Array("Apple", "Banana", "Mango");
  ```

### Accessing Elements
You can access elements in an array using their index:
```javascript
let firstFruit = fruits[0];  // "Apple"
let secondFruit = fruits[1]; // "Banana"
```

### Modifying Elements
You can modify elements by directly assigning a new value to a specific index:
```javascript
fruits[1] = "Orange";
console.log(fruits); // ["Apple", "Orange", "Mango"]
```

### Common Array Methods
- **`push()`**: Adds a new element to the end of the array.
  ```javascript
  fruits.push("Grapes");
  // ["Apple", "Orange", "Mango", "Grapes"]
  ```

- **`pop()`**: Removes the last element from the array.
  ```javascript
  let lastFruit = fruits.pop(); 
  // "Grapes", fruits = ["Apple", "Orange", "Mango"]
  ```

- **`shift()`**: Removes the first element from the array.
  ```javascript
  let firstFruit = fruits.shift();
  // "Apple", fruits = ["Orange", "Mango"]
  ```

- **`unshift()`**: Adds a new element to the beginning of the array.
  ```javascript
  fruits.unshift("Pineapple");
  // ["Pineapple", "Orange", "Mango"]
  ```

- **`length`**: Returns the number of elements in an array.
  ```javascript
  let numberOfFruits = fruits.length;
  // 3
  ```

- **`indexOf()`**: Returns the first index of a specified element, or `-1` if the element is not found.
  ```javascript
  let index = fruits.indexOf("Mango");
  // 2
  ```

- **`splice()`**: Adds or removes elements from an array.
  ```javascript
  fruits.splice(1, 1); // Removes 1 element at index 1
  // ["Pineapple", "Mango"]
  
  fruits.splice(1, 0, "Banana"); // Adds "Banana" at index 1
  // ["Pineapple", "Banana", "Mango"]
  ```

- **`slice()`**: Returns a new array with selected elements from the original array.
  ```javascript
  let citrus = fruits.slice(1, 3);
  // ["Banana", "Mango"]
  ```

### Iterating Over an Array
You can loop through an array using `for`, `forEach`, `for...of`, and other loops:
```javascript
for (let i = 0; i < fruits.length; i++) {
    console.log(fruits[i]);
}

fruits.forEach(function(item, index) {
    console.log(index, item);
});

for (let fruit of fruits) {
    console.log(fruit);
}
```
