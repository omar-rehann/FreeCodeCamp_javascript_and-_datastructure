# Pyramid Pattern Generator

This project is a simple JavaScript code that prints a pyramid shape using characters.

## How it works
- The pyramid is built using the character `#`.
- You can control the height of the pyramid using the variable `count`.
- The variable `inverted` decides whether the pyramid is printed normally or upside down.
- Each row is generated using the `padRow` function and stored in the `rows` array, then joined into the final `result`.
## Output
       #       
      ###      
     #####     
    #######    
 


.

## Code

```js
const character = "#";
const count = 8;
const rows = [];
let inverted = true;

function padRow(rowNumber, rowCount) {
    return " ".repeat(rowCount - rowNumber) + character.repeat(2 * rowNumber - 1) + " ".repeat(rowCount - rowNumber);
}

for (let i = 1; i <= count; i++) {
    if (inverted) {
        rows.unshift(padRow(i, count));
    } else {
        rows.push(padRow(i, count));
    }
}

let result = ""

for (const row of rows) {
    result = result + row + "\n";
}

console.log(result) 
