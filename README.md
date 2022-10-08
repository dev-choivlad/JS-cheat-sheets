# JS-cheat-sheets
Java script cheat sheets. All methods at fingertips.  
### Strings methods  
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

" Hello ".trimSrart() // "Hello "

" Hello ".trimEnd() // " Hello"
```
