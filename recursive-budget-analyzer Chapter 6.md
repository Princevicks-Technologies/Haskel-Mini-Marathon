
# 💸 Recursive Budget Analyzer – Mini Console Project

You’ve just completed Chapter 6, where you unlocked the power of recursion and folds in Haskell:

✅ Why recursion is core to Haskell  
✅ Thinking recursively – breaking down problems into base & recursive steps  
✅ Recursive patterns: sum, product, and, length, reverse, drop, take, map, filter  
✅ Steps to create your own recursive function  
✅ Extracting the `foldr` pattern  
✅ The `foldl` and `foldl'` functions  
✅ Choosing the right fold for performance and clarity  

This mini-marathon challenges you to build a **console-based Recursive Budget Analyzer**. You’ll process daily income and expense records using custom recursion and folds.

---

## 🎯 Objectives

🔁 Use recursion to define list-processing functions:  
Implement custom versions of `sum`, `filter`, `map`, `reverse`, and more.

💡 Think recursively:  
Break list operations into base and recursive steps.

🧩 Use pattern matching to deconstruct and process transactions.

⚖️ Apply `foldr`, `foldl`, and `foldl'`:  
Aggregate totals and reverse lists efficiently.

🔍 Build modular pure functions:
- `sumIncome :: [Int] -> Int`  
- `sumExpenses :: [Int] -> Int`  
- `filterExpenses :: [Int] -> [Int]`  
- `reverseHistory :: [Int] -> [Int]`

🧪 Practice defensive design:  
Use safe versions (e.g., `Maybe`) where necessary for filtering and mapping.

---

## 🧪 What to Deliver

A runnable console app that:

🔹 Displays a welcome message and simple menu:

```
Welcome to Recursive Budget Analyzer!
1. Add transaction
2. Show transactions
3. Analyze budget
4. Exit
```

🔹 Uses pattern matching to route commands.

🔹 Accepts multiple transactions as integers:  
Positive = income, Negative = expense

🔹 Calculates:
- Total income
- Total expenses
- Balance

🔹 Uses your own versions of:
- `sum`, `filter`, `map`, `reverse`

🔹 Displays reversed transaction history using recursion.

---

## 💡 Bonus Challenges

⭐ Use `Maybe` to safely filter out invalid inputs (e.g., `filterValid :: [Int] -> Maybe [Int]`)

📂 Add basic file I/O to save and load transaction history.

🧾 Model transactions using:

```haskell
data Transaction = Transaction { amount :: Int, note :: String }
```

👨‍💻 Use tuples for reporting:

```haskell
("Total Income", 1200), ("Total Expenses", 500)
```

---

## 📦 Build Instructions

✅ Run and test in **GHCi**  
🗂 Organize code into reusable functions inside a single `Main` module  
📦 Optional: Package with **Stack** or **Cabal**  

📃 Include a small `README.md` describing:
- What the app does  
- How to run it  
- Sample input/output
