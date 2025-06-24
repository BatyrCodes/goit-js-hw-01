# JavaScript Practice Tasks

A simple HTML + JavaScript project with three beginner-level tasks. This setup is great for practicing function creation, working with numbers and strings, and understanding basic browser output using `console.log()`.

---

## 📁 Project Structure

project/
├── index.html
└── js/
├── task-1.js
├── task-2.js
└── task-3.js

yaml
Копировать
Редактировать

---

## 🚀 How to Run

1. Clone or download the repository.
2. Open `index.html` in your browser.
3. Open the browser's **Console** (F12 or right-click → Inspect → Console tab) to see the output of the JavaScript functions.

---

## 📌 Tasks Overview

### ✅ Task 1 — `makeTransaction(quantity, pricePerDroid)`

**File:** `js/task-1.js`

This function calculates the total cost of ordering a certain number of droids and returns a message with the result.

**Function Logic:**

```js
function makeTransaction(quantity, pricePerDroid) {
  return `You ordered ${quantity} droids worth ${quantity * pricePerDroid} credits!`;
}
Examples:

js
Копировать
Редактировать
makeTransaction(5, 3000); // "You ordered 5 droids worth 15000 credits!"
makeTransaction(3, 1000); // "You ordered 3 droids worth 3000 credits!"
✅ Task 2 — getShippingMessage(country, price, deliveryFee)
File: js/task-2.js

This function returns a message showing the total cost of shipping to a given country (product price + delivery fee).

Function Logic:

js
Копировать
Редактировать
function getShippingMessage(country, price, deliveryFee) {
  return `Shipping to ${country} will cost ${price + deliveryFee} credits`;
}
Examples:

js
Копировать
Редактировать
getShippingMessage("Australia", 120, 50); // "Shipping to Australia will cost 170 credits"
getShippingMessage("Germany", 80, 20);    // "Shipping to Germany will cost 100 credits"
✅ Task 3 — getElementWidth(content, padding, border)
File: js/task-3.js

This function calculates the total width of an HTML element based on its content width, padding, and border.

The function removes "px", converts to numbers using parseFloat(), and assumes that padding and border are on both sides (left + right).

Function Logic:

js
Копировать
Редактировать
function getElementWidth(content, padding, border) {
  const contentWidth = parseFloat(content);
  const paddingWidth = parseFloat(padding) * 2;
  const borderWidth = parseFloat(border) * 2;
  return contentWidth + paddingWidth + borderWidth;
}
Examples:

js
Копировать
Редактировать
getElementWidth("50px", "8px", "4px");     // 74
getElementWidth("60px", "12px", "8.5px");  // 101
getElementWidth("200px", "0px", "0px");    // 200
🧠 What You Learn
Writing and calling functions

String interpolation with template literals

Basic math operations in JavaScript

Parsing numeric values from strings (parseFloat)

How HTML <script defer> works for loading JS files

