\# 🎓 Student Profile Manager – Mini Console Project

You’ve just completed \*\*Chapter 8\*\*, where you explored how to design and organize your own \*\*types\*\* in Haskell:

✅ Type synonyms    
✅ New types with \`data\`    
✅ Creating and using types    
✅ Value parameters    
✅ Record syntax  

This mini-marathon challenges you to build a \*\*command-line Student Profile Manager\*\*. You’ll design and manipulate structured student data using type synonyms, record syntax, and custom types.

\---

\#\# 🎯 Objectives

Define and use \*\*type synonyms\*\* – simplify types like \`Name\`, \`StudentID\`, and \`CGPA\`.

Create \*\*custom data types\*\* using \`data\` – define a \`Student\` record with named fields.

Use \*\*record syntax\*\* – access and update fields clearly and expressively.

Apply \*\*value parameters\*\* – explore polymorphic record types for reusable structures.

Design a clear menu-based flow – organize input/output using pure and interactive functions.

Encourage \*\*modular thinking\*\* – structure logic across clean, reusable functions:

\`\`\`haskell  
addStudent :: IO Student    
showStudents :: \[Student\] \-\> IO ()    
searchByID :: \[Student\] \-\> IO ()    
updateCGPA :: \[Student\] \-\> IO \[Student\]  
\`\`\`

\---

\#\# 🧪 What to Deliver

A runnable console app that:

📢 Displays a welcome message and main menu:

\- Add Student    
\- Show All Students    
\- Search by ID    
\- Update CGPA    
\- Exit  

✅ Uses \*\*type synonyms\*\* to clarify function signatures    
✅ Defines a \`Student\` data type using \*\*record syntax\*\*    
✅ Accepts user input and stores student records in memory    
✅ Uses pattern matching and list functions to process data    
✅ Clearly separates concerns using helper functions  

\---

\#\# 💡 Bonus Challenges

🔁 Add the ability to delete a student by ID.

📁 Use file I/O (\`readFile\`, \`writeFile\`) to save and load student data.

🧬 Define a \*\*generic record\*\* using value parameters:

\`\`\`haskell  
data Record a \= Record { recordId :: Int, content :: a }  
\`\`\`

📋 Nest a \`Course\` type inside each student for advanced tracking.

🔐 Use modules to hide internal data and expose access functions only.

\---

\#\# 📦 Build Instructions

🧪 Run and test in \*\*GHCi\*\*

📁 Organize logic into functions inside a \`Main.hs\` module

📦 Optional: Package with \*\*Stack\*\* or \*\*Cabal\*\*

📄 Include a \`README.md\` with:

\- What the app does    
\- How to run it    
\- Sample inputs and outputs  

