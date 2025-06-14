# 🧹 Saturday Chore Simulator

Welcome to the Summer Chore Simulator! This project is a hands-on demonstration of asynchronous JavaScript programming using three different methods: **Callbacks**, **Promises**, and **Async/Await**. Each version simulates a series of Saturday chores that must be completed in order — unless someone gets too tired and falls asleep on the job. 😴

---

## ✅ Completed Version: Callbacks

### `callbackVersion.js`

This version uses classic callback functions and simulates the perils of **callback hell**. The simulation includes:

- A strict chore routine:
  1. Mow the yard (can’t fall asleep here — caffeine levels still maxed).
  2. Weed eat the edges.
  3. Trim the hedges.
  4. Collect firewood.
  5. Water the garden.

- A random chance of the person falling asleep after each task (except the first), which prevents them from completing the rest of the chores.

- A single entry point function, `doSummerChores(name)`, that kicks off the whole routine.

### Example Output

```bash
Jill mowed the yard.
Jill finished using the weed eater.
Jill finished trimming the hedges.
Jill fell asleep after trimming the hedges.
```

Or, if you're lucky:

```bash
Jill mowed the yard.
Jill finished using the weed eater.
Jill finished trimming the hedges.
Jill finished collecting wood.
Jill finished watering the garden.
Jill finished all their chores!
```

---

## 🛠 In Progress

- `promiseVersion.js` – Coming soon! We'll rewrite the routine using Promises to flatten out that pyramid of doom. ⛺
- `asyncAwaitVersion.js` – Coming after Promises. Because chores are better when they await your attention politely. 🕰️

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
```

Once the other versions are completed, you can try:

```bash
node promiseVersion.js
node asyncAwaitVersion.js
```

---

## 📁 File Structure

```
├── callbackVersion.js       // Callback-based chore routine
├── promiseVersion.js        // Promise-based version (coming soon)
├── asyncAwaitVersion.js     // Async/Await version (coming soon)
└── README.md                // You're looking at it!
```

---

## 📚 Fun Fact

No actual humans were forced to mow virtual lawns in the making of this program. But we *did* make JavaScript sweat a little.

---