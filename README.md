# JS-cheat-sheets
Java script cheat sheets. All methods at fingertips.  
### String methods  
```javascript
"Hello".charAt(4) // o

"Hello".search("l") // 2 (returns the position at which the match is located, or -1 if there are no matches.)

"Hello".indexOf("l") // 2 (returns the position at which the match is located, or -1 if there are no matches.)

"Hello".lastIndexOf("l") // 3 (same as indexOf(), but the search starts from the end of the string)

"Hello".includes("e") // true

"Hello".startsWith("H") // tru

"Hello".endsWith("H") // false

"Hello".slice(1, 3) // el (returns substring from start to end, but not including end)

"Hello".substring(1, 3) // el (same as slice(), start/end can be set to negative values.)

"Hello".substr(1, 3) // ell (returns substring from start with number of chars equal to lenght)

"Hello".match(/[A-Z]/g) // ["H"]

"Hello".concat("", "World") // Hello World

"Hello".toLowerCase() // hello

"Hello".toUpperCase() // HELLO

"Hello".replace("llo", "y") // Hey

"Hello".repeat(2) // HelloHello

"Hello".split("") // ["H", "e", "l", "l", "o"]

" Hello ".trim() // "Hello"

" Hello ".trimStart() // "Hello "

" Hello ".trimEnd() // " Hello"
```
### Array methods
```javascript
[1, 2, 3].push(4) // [1, 2, 3, 4]
  
[1, 2, 3].pop() // [1, 2]

[1, 2, 3].unshift(0) // [0, 1, 2, 3]

[1, 2, 3].shift() // [2, 3]

[1, 2, 3].reverse() // [3, 2, 1]
  
[1, 2, 3].splice(0, 1, true) // [true, 2, 3] 
// It modifies arr starting from the index start: removes deleteCount elements and then inserts elem1, ..., elemN at their place. 
// Returns the array of removed elements.

[1, 2, 3].slice(0, 2) // new array [1, 2]
//Returns a new array copying to it all items from index start to end (not including end).

[1, 2, 3].slice() // new copy of the array [1, 2, 3]
// Calling without arguments: arr.slice() creates a copy of the arr

[1, 2, 3].concat([4, 5]) // [1, 2, 3, 4, 5]
// returns a new array containing items from arr, then arg1, arg2 etc.

[1, 2, 3].forEach(function(item, index, array) {
  // runs a function for every element of the array.
})

[1, 2, 3].indexOf(2, 1) // 1
// Looks for item starting from index from, and returns the index where it was found, otherwise -1.

[1, 2, 3].lastIndexOf(2, 1) // 1
// Same as infexOf(), but searches from right to left.

[1, 2, 3].includes(3, 0) // true
// Looks for item starting from index from, returns true if found.

[
  {id: 1, name: "Gagarin"},
  {id: 2, name: "Armstrong"},
  {id: 3, name: "Jemison"}
].find(item => item.id == 1) // {id: 1, name: "Gagarin"}
// If true, item is returned and iteration is stopped
// if false, returns undefined

[
  {id: 1, name: "Gagarin"},
  {id: 2, name: "Armstrong"},
  {id: 3, name: "Jemison"}
].filter(item => item.id < 3) // [{id: 1, name: "Gagarin"}, {id: 2, name: "Armstrong"}]
// If true, item is pushed to results and the iteration continues
// returns an array of all matching elements
// returns empty array if nothing found

[1, 2, 3].map(item => item + 1) // [2, 3, 4]
// Returns a new array from calling a function for every array elements

[4, 1, 2, 3].sort((a, b) => {return a - b}) // [1, 2, 3, 4]
// Sorts the array in place, changing its element order.

[1, 2, 3].reverse() // [3, 2, 1]

[1, 2, 3].join(", ") // "1, 2, 3"

[1, 2, 3].reduce((sum, current) => sum + current, 0) // 6
// Function is applied to all array elements one after another and “carries on” its result to the next call.
// Calculation flow:
// the 1st call: sum is 0, current is 1, result is 1
// the 2nd call: sum is 1, current is 2, result is 3
// the 3rd call: sum is 3, current is 3, result is 6

Array.isArray([1, 2, 3]) // true

```
