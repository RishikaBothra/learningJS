# Interesting stuff is here


`// print only Odd numbers from arr`
```javascript
function isOdd(num) {
    if (num === 0) {
        return "Zero is not defined"
    } else {
        if (num % 2 === 0) {
            return false
        } else {
            return true
        }
    }
}

let arr = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];


for (let i = 0; i < arr.length; i++) {

	if (isOdd(arr[i])) {
		console.log(arr[i])
	}

}
```