
# 🎓 Type-Savvy Calculator – Mini Console Project

You’ve just completed **Chapter 7**, where you explored the awesomeness of **type classes** in Haskell:

✅ What are type classes  
✅ Common type classes: `Eq`, `Ord`, `Num`, `Integral`, `Floating`, `Read`, `Show`  
✅ The most general valid types  
✅ Multiple constraints

This mini-marathon challenges you to build a **type-driven calculator** that demonstrates how Haskell uses type classes to support polymorphism, comparisons, string conversions, and numerical operations — all in a clean, type-safe way.

---

## 🎯 Objectives

🔢 **Use `Eq` and `Ord`** – compare two values for equality and ordering  
🧮 **Use `Num`, `Integral`, and `Floating`** – perform arithmetic with multiple number types  
🔡 **Use `Read` and `Show`** – convert between strings and values cleanly  
🧰 **Write polymorphic functions** – use type variables and constraints  
🔗 **Use multiple constraints** – require more than one type class per function  
💡 **Explore generality** – write the most flexible functions possible using valid constraints

Encourage modular thinking – split logic across expressive functions:

```haskell
compareValues :: (Eq a, Ord a) => a -> a -> String
performOperation :: (Num a, Show a) => String -> a -> a -> String
parseInput :: Read a => String -> a
```

---

## 🧪 What to Deliver

A runnable console app that:

📢 Displays a welcome message and menu:

- Compare Values  
- Perform Operation  
- Parse from String  
- Convert to String  
- Exit

🧠 Uses type class constraints in function signatures  
⚖️ Performs comparisons like `a == b`, `a > b`  
➕ Performs arithmetic like `a + b`, `a * b`, only if `Num`  
🔄 Uses `Read` and `Show` to convert between string and numeric types  
🔤 Allows both `Int` and `Float` inputs

---

## 💡 Bonus Challenges

🚫 Handle invalid `Read` inputs using `Maybe` or `Either`  
🧩 Define a custom data type (e.g., `MyNumber`) and make it an instance of `Eq`, `Ord`, and `Show`  
📁 Add basic file I/O to save and read operations performed  
🛠️ Provide clear type signatures for all user-defined functions  
🎯 Demonstrate multiple constraints in one or more functions

---

## 📦 Build Instructions

- Run and test in **GHCi**  
- Organize code into modular functions (in `Main.hs`)  
- Optional: Package with **Stack** or **Cabal**  
- Include a small `README.md` describing:
  - What the app does  
  - How to run it  
  - Sample inputs and outputs  
