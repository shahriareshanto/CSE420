# CSE420 Compiler Design Lab – Lexical & Syntax Analyzer

This project is part of the CSE420 (Compiler Design) Lab at BRAC University. It implements a basic compiler front-end using **Lex** and **Yacc** to perform lexical analysis, syntax analysis, and symbol table management.

---

## 📂 Files Included
- `lex.l`: Tokenizer using Flex (Lex)
- `syntax.y`: Grammar-based parser using YACC
- `symbol_info.h`, `symbol_table.cpp`: Symbol table and scope management
- `input.txt`: Sample test input
- `output.txt`: Output file (student ID based)
- `README.md`: This file

---

## ⚙️ How to Compile and Run
```bash
flex lex.l
yacc -d syntax.y
g++ y.tab.c lex.yy.c symbol_table.cpp -o parser
./parser < input.txt
