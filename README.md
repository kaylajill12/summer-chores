# 🧹 Summer Chore Simulator

Welcome to the Summer Chore Simulator! This project is a hands-on demonstration of asynchronous JavaScript programming using three different methods: **Callbacks**, **Promises**, and eventually **Async/Await**. The scenario involves a person working through a list of summer chores every Saturday — with the chance of getting too tired and falling asleep before completing them all. (Chore fatigue is real.)

## 📋 The Chore List (in strict order)

1. Mow the yard – 2000ms  
2. Weed eat the edges – 1500ms  
3. Trim the hedges – 1000ms  
4. Collect fallen wood – 2500ms  
5. Water the garden – 500ms  

If the person stays awake through all chores, they complete their list successfully. If they fall asleep mid-task, the program stops execution and logs an appropriate message.

---

## ✅ Completed Versions

### 1. `callbackVersion.js`
- Demonstrates classic **callback-based** asynchronous flow.
- Each chore function accepts a `name` and a `callback`.
- Chores are executed in a nested callback chain — a.k.a. "callback hell."
- Introduces potential sleepiness using `Math.random()` to simulate fatigue after each chore (except mowing, which is always completed first).

### 2. `promiseVersion.js`
- Refactors all chore functions to return **Promises** instead of using callbacks.
- Uses `.then()` chaining to sequence chores in a clean, linear fashion.
- A single `.catch()` handles any "I fell asleep" cases and logs the point of failure.
- Greatly improves readability and flow control over the callback version.

---

## 🚧 Upcoming: `asyncAwaitVersion.js`
- The final version will convert the Promise-based implementation into a fully async/await structure.
- Will further simplify error handling and task sequencing using modern JavaScript syntax.
- To be updated once implemented!

---

## 💡 Purpose

This project was created to practice:
- Writing and managing asynchronous code in JavaScript
- Understanding the difference between callbacks, promises, and async/await
- Handling flow control and error simulation (i.e., falling asleep) in a real-world-style scenario

---

## 🚀 Usage

Run each version using Node.js in your terminal:

```bash
node callbackVersion.js
node promiseVersion.js
```

Once the other version is completed, you can try:

```bash
node asyncAwaitVersion.js
```

Each run randomly determines if the person gets tired mid-task, so results may vary!

---

## 📁 File Structure

```
├── callbackVersion.js       // Callback-based chore routine
├── promiseVersion.js        // Promise-based version
├── asyncAwaitVersion.js     // Async/Await version (coming soon)
└── README.md                // You're looking at it!
```

---

## 📚 Fun Fact

No actual humans were forced to mow virtual lawns in the making of this program. But we *did* make JavaScript sweat a little.

---