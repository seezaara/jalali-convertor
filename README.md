# Jalaali JavaScript

fastest javascript functions for converting Jalaali (Jalali, Persian, Khayyami, Khorshidi, Shamsi) and Gregorian calendar systems to each other.

## Usage

```js
const date = require("jalali-convertor")

// get curent date
console.log(date.jDate()); // [ 1402, 3, 4 ]
console.log(date.gDate()); // [ 2023, 5, 25 ]

// get curent timestamp
console.log(date.jTime()); // 1685018686260
console.log(date.gTime()); // 1685018686261
console.log(new Date(date.jTime())); // 2023-05-25T12:44:46.262Z UTC
console.log(new Date(date.gTime())); // 2023-05-25T12:44:46.262Z UTC

// get specific date
console.log(date.jDate(1685014909046)); // [ 1402, 3, 4 ]
console.log(date.gDate(1685014909046)); // [ 2023, 5, 25 ]

// get specific timestamp
console.log(date.jTime(1402, 3, 4)); // 1684960200000
console.log(date.gTime(2023, 5, 25)); // 1684960200000
console.log(new Date(date.jTime(1402, 3, 4))); // 2023-05-24T20:30:00.000Z UTC
console.log(new Date(date.gTime(2023, 5, 25))); // 2023-05-24T20:30:00.000Z UTC

// get specific timestamp at 13:30 in your time zone
console.log(date.jTime(1402, 3, 4, 13, 30)); // 1685008800000
console.log(date.gTime(2023, 5, 25, 13, 30)); // 1685008800000
console.log(new Date(date.jTime(1402, 3, 4, 13, 30))); //2023-05-25T10:00:00.000Z UTC
console.log(new Date(date.gTime(2023, 5, 25, 13, 30))); //2023-05-25T10:00:00.000Z UTC

// convert date
console.log(date.j2g(1402, 3, 4)); // [ 2023, 5, 25 ]
console.log(date.g2j(2023, 5, 25)); // [ 1402, 3, 4 ]

```
# licence
 <p>
    <img width="32px" src="https://raw.githubusercontent.com/seezaara/RocketV2ray/main/doc/logo.png"><a href="https://www.youtube.com/@seezaara">created by seezaara</a>
</p> 









