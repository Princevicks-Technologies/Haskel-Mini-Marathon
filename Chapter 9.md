\# 🎓 Contact Book – Mini Console Project (Chapter 9\)

Build a command-line \*\*Contact Book\*\* app using Chapter 9 concepts:

✅ Parameterized types and synonyms    
✅ Recursive data types    
✅ \`newtype\` for clarity and safety    
✅ Kind awareness (\`\*\`, \`\* \-\> \*\`)  

\---

\#\# 🎯 Objectives

\- Use \`newtype\` for \`Name\`, \`PhoneNumber\`, \`Email\`, \`ContactID\`    
\- Create a \*\*parameterized Contact type\*\*:    
  \`\`\`haskell  
  data Contact a \= Contact { contactId :: ContactID, contactName :: Name, contactInfo :: a }  
  \`\`\`  
\- Define optional \*\*recursive list\*\* for contacts:    
  \`\`\`haskell  
  data ContactList a \= Empty | Node (Contact a) (ContactList a)  
  \`\`\`  
\- Understand \*\*kinds\*\* with parameterized types    
\- Clean modular functions for adding, showing, searching contacts  

\---

\#\# 🧪 Features to Build

\- Menu: Add, View, Search, Update, Exit    
\- Store contacts with parameterized \`Contact a\`    
\- Use recursive structures to manage contact list    
\- Show output using custom formatting  

\---

\#\# 💡 Bonus

\- Add file saving/loading    
\- Search by partial name    
\- Allow editing of contact info    
\- Use tuples or records for extended info    
\- Modularize and expose only necessary functions  

\---

\#\# 📦 Build Instructions

\- Run in \*\*GHCi\*\*    
\- Organize in \`Main.hs\`    
\- Add \`README.md\` with what it does, how to run, sample output  

