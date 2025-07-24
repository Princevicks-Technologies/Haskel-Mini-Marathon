
# 🧠 Haskell Mini Marathon – Task Manager with Higher-Order Functions

You’ve just completed **Chapter 7**, where you unlocked powerful Haskell abstractions using **higher-order functions** and **function composition**. Now it’s time to apply what you’ve learned in a real-world scenario.

This mini-marathon challenges you to build a **functional Task Manager** using core concepts like `filter`, `any`, lambdas, curried functions, partial application, and function composition.

---

## 🎯 Project Objective

To build a command-line **Task Manager** in Haskell that can:

- Filter tasks by status or priority  
- Search tasks using custom criteria  
- Compose and apply functions elegantly  
- Practice point-free and partially applied functions

---

## 📚 Concepts to Apply

### ✅ Higher-order functions

Use functions like `filter`, `map`, `foldr`, and `any` to process task lists.

### ✅ `filter`

Filter tasks that are incomplete:

```haskell
incompleteTasks = filter (not . done) tasks
```

### ✅ `any`

Check if any task is marked as urgent:

```haskell
hasUrgent = any urgent tasks
```

### ✅ Lambda functions

Use inline lambdas for quick operations:

```haskell
filter (	 -> priority t == "High") tasks
```

### ✅ Precedence and Associativity

Understand how expressions like `f $ g x` work without parentheses.

```haskell
print $ map show tasks
```

### ✅ Curried Functions & Partial Application

Build reusable filters like:

```haskell
filterByPriority :: String -> [Task] -> [Task]
filterByPriority p = filter (	 -> priority t == p)
```

### ✅ Applying and Composing Functions

Chain behaviors together:

```haskell
processTasks = map show . filter (not . done)
```

### ✅ `$` Operator

Simplify function application:

```haskell
print $ filter urgent tasks
```

### ✅ `.` Operator

Compose small functions:

```haskell
taskTitles = map (title . toUpperCase)
```

### ✅ Point-Free Style

Write clean code without arguments:

```haskell
filterIncomplete = filter (not . done)
```

---

## 🧪 What to Deliver

A runnable console application that:

- Defines a `Task` data type with `title`, `done :: Bool`, `priority :: String`
- Allows filtering tasks using higher-order functions
- Demonstrates use of `filter`, `any`, lambdas, and composition
- Has at least 2 point-free functions
- Uses both `$` and `.` operators clearly

---

## 💡 Bonus Challenges

⭐ Add a search function using `any` and `words`  
⭐ Use `foldr` to count completed tasks  
⭐ Support partial application for priority filters  
⭐ Use a list comprehension and then refactor it into point-free

---

## 📦 Build Instructions

✅ Run in **GHCi** (`ghci TaskManager.hs`)  
✅ Use pure functions in a modular way  
✅ Keep logic clean and reusable  
✅ Include a `README.md` explaining:
- Features  
- Example commands  
- Key Haskell concepts used  
