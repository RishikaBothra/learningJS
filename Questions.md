# Questions of JS

1. **Sum of Array Elements**:
   - Write a function `sumArray(arr)` that takes an array of numbers as input and returns the sum of all the elements in the array. Use a loop to iterate through the array.

2. **Factorial Calculation**:
   - Create a function `factorial(n)` that returns the factorial of a given number `n`. Use a loop and conditional statements to calculate the factorial.
```javascript


function factorial(n)
{
    let ans=n
    for(let i=n-1;i>=1;i--)
    {
        ans= ans*i

    }
    return ans
}
let result = factorial(5)
console.log(result);
```
3. **Palindrome Check**:
   - Write a function `isPalindrome(str)` that checks if a given string is a palindrome (reads the same forward and backward). Use conditional statements to compare characters.

4. **Fibonacci Sequence**:
   - Implement a function `fibonacci(n)` that returns the first `n` numbers of the Fibonacci sequence. Use loops to generate the sequence.

5. **Odd or Even**:
   - Write a function `isEven(num)` that takes a number as input and returns `true` if the number is even, and `false` if it’s odd. Use a conditional statement to check the parity.
``` javascript
function iseven(num)
      {

    if(num%2===0){
        return true
    }
    else{
        return false
    }

      }
    let result= iseven(5)
    console.log(result);
```

6. **Prime Number Checker**:
   - Create a function `isPrime(num)` that checks if a number is a prime number. Use loops and conditional statements to determine if the number has any divisors other than 1 and itself.
```javascript
function isprime(num)
{
  if(num<=1)
    return false;
    if(num===2)
      return true;
    if(num===3)
      return true;
    if(num===5)
      return true;
    if(num%2===0)
      return false;
    if(num%3===0)
      return false;
    for(let i=5;i*i<=num;i=i+6){
      if(num%i===0)
        return false;
    }
    
    return true;
  
}
console.log(isprime(29));
```

7. **Counting Vowels in a String**:
   - Write a function `countVowels(str)` that counts the number of vowels (`a`, `e`, `i`, `o`, `u`) in a given string. Use a loop to iterate through the string and a conditional statement to check for vowels.
```javascript
function countvowels(str)
{
  const vowels='aeiouAEIOU'
  let count= 0;
  for( let i=0;i<str.length; i++){
  if (vowels.includes(str[i]))
  {count++;} }
  return count;

}
console.log(countvowels("hey there"));
```

8. **Reversing a String**:
   - Implement a function `reverseString(str)` that takes a string as input and returns the reversed string. Use a loop to reverse the string character by character.
```javascript
function reverseString(str) {
  
  let reversed = '';
  for (let i = str.length - 1; i >= 0; i--) {
    
    reversed = reversed+ str[i];
  }
  return reversed;
}
console.log(reverseString("hey there!"));
```


9. **Maximum and Minimum in Array**:
   - Write a function `findMaxMin(arr)` that takes an array of numbers and returns both the maximum and minimum values in the array. Use loops and conditional statements to find these values.
```javascript

function findmaxmin(arr)
{
  if (arr.length===0){
    return{ max: null, min:null};
}
let max =arr[0];
let min= arr[0];
for (let i= 0; i< arr.length;i++)
{
  if(arr[i] > max)
  {
    max=arr[i]
  }
  if(arr[i] < min)
  {
    min=arr[i]
  }
}
return{max:max, min:min};
}
let inputarr =[2, 6, 7, 8];

console.log(findmaxmin(inputarr)) 
```

10. **FizzBuzz**:
    - Create a function `fizzBuzz(n)` that prints numbers from 1 to `n`. For multiples of 3, print "Fizz"; for multiples of 5, print "Buzz"; and for multiples of both 3 and 5, print "FizzBuzz". Use loops and conditional statements.
```javascript
function fizzbuzz(n)
{
  
  if(n%3===0)
    console.log(" fizz");
  if(n%5==0)
    console.log("buzz");
  if(n%5===0&&n%3===0)
    console.log("fizzbuzz");
}
console.log(fizzbuzz(15));
```

