
# 🎓 GP Calculator – Mini Console Project

You’ve just completed **Chapter 4**, where you explored the power of **pattern matching** in Haskell:

✅ Pattern matching in functions  
✅ Catch-all patterns  
✅ Closer look at lists  
✅ Lists and tuples  
✅ Case expressions  
✅ Declaration style vs. expression style  

This mini-marathon challenges you to build a **command-line GP Calculator**. You’ll collect student course scores and compute the **Grade Point Average (GPA)**, making full use of Haskell’s expressive features.

---

## 🎯 Objectives

🔹 **Use pattern matching in function definitions** – process user input like course scores and grades with clear, readable branches.

🔹 **Design expressive data types** – model courses using tuples, records, or even custom data types.

🔹 **Apply catch-all patterns safely** – handle invalid or unexpected inputs without crashing your app.

🔹 **Practice case expressions** – convert raw scores to letter grades or grade points using case expressions.

🔹 **Work with list patterns** – map over course lists, extract information, and compute GPA using folds or recursion.

🔹 **Contrast declaration vs. expression styles** – implement one module using `let/in` declarations and another using inline expressions.

🔹 **Encourage modular thinking** – split your logic across pure, reusable functions like:

```haskell
scoreToGrade :: Int -> String
gradeToPoint :: String -> Float
calculateGPA :: [(String, Int)] -> Float
```

---

## 🧪 What to Deliver

A **runnable console application** that:

📌 Displays a welcome message and menu:
```
1. Enter Course  
2. Show All  
3. Calculate GPA  
4. Exit
```

📌 Uses **pattern matching** to route user commands.

📌 Accepts multiple course names and scores (e.g., `("Math", 78)`).

📌 Converts raw scores to **letter grades** and **grade points** using `case` expressions.

📌 Calculates GPA using **list transformations** and **tuples**.

📌 Outputs:
- A table showing each course, score, letter grade, and point.
- Final calculated GPA (to two decimal places).

---

## 💡 Bonus Challenges

⭐ Use `Maybe` when converting scores to grades – handle out-of-bound scores gracefully.  
⭐ Add **file I/O** to save and load the course list.  
⭐ Define a custom data type:
```haskell
data Course = Course { name :: String, score :: Int }
```
⭐ Use tuples for `(Grade, GradePoint)` and pattern match accordingly.

---

## 📦 Build Instructions

✅ Run and test in **GHCi** (`ghci GPCalculator.hs`)  
✅ Organize your code into **pure functions** inside a `Main` module  
✅ Optional: Package using **Stack** or **Cabal**  
✅ Include a small `README.md` file with:
- What the app does  
- How to run it  
- Sample inputs and outputs  
