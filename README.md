# JavaScript Practice Tasks

A simple HTML + JavaScript project with three beginner-level tasks. This setup is ideal for practicing function creation, working with numbers and strings, and understanding how to view JavaScript output using `console.log()` in the browser.

---

## 📁 Project Structure

project/
├── index.html
└── js/
├── task-1.js
├── task-2.js
└── task-3.js


## 🚀 How to Run

1. Clone or download the repository.
2. Open `index.html` in your browser.
3. Open the browser's **Console** (press `F12` or right-click → Inspect → Console tab) to see the output of the JavaScript functions.

---

## 📌 Tasks Overview

### ✅ Task 1 — `makeTransaction(quantity, pricePerDroid)`

**File:** `js/task-1.js`  
This function calculates the total cost of ordering a certain number of droids and returns a message with the result.

```js
function makeTransaction(quantity, pricePerDroid) {
  return `You ordered ${quantity} droids worth ${quantity * pricePerDroid} credits!`;
}
Examples:
makeTransaction(5, 3000); // "You ordered 5 droids worth 15000 credits!"
makeTransaction(3, 1000); // "You ordered 3 droids worth 3000 credits!"
makeTransaction(10, 500); // "You ordered 10 droids worth 5000 credits!"

✅ Task 2 — getShippingMessage(country, price, deliveryFee)
File: js/task-2.js
This function returns a message showing the total shipping cost, including product price and delivery fee.

function getShippingMessage(country, price, deliveryFee) {
  return `Shipping to ${country} will cost ${price + deliveryFee} credits`;
}
Examples:
getShippingMessage("Australia", 120, 50); // "Shipping to Australia will cost 170 credits"
getShippingMessage("Germany", 80, 20);    // "Shipping to Germany will cost 100 credits"
getShippingMessage("Sweden", 100, 20);    // "Shipping to Sweden will cost 120 credits"

✅ Task 3 — getElementWidth(content, padding, border)
File: js/task-3.js
This function calculates the full width of an HTML element by adding content width, horizontal padding, and border values.

It parses numeric values from strings with px using parseFloat() and assumes padding and border are applied on both sides.

function getElementWidth(content, padding, border) {
  const contentWidth = parseFloat(content);
  const paddingWidth = parseFloat(padding) * 2;
  const borderWidth = parseFloat(border) * 2;
  return contentWidth + paddingWidth + borderWidth;
}
Examples:
getElementWidth("50px", "8px", "4px");     // 74
getElementWidth("60px", "12px", "8.5px");  // 101
getElementWidth("200px", "0px", "0px");    // 200
🧠 What You'll Learn
Writing and calling functions

String interpolation with template literals

Basic math operations in JavaScript

Parsing numeric values from strings using parseFloat()

Understanding how <script defer> works in HTML

