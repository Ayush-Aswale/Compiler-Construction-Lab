# Compiler Construction Laboratory

This repository contains practical laboratory implementations for the **Compiler Construction / Compiler Design** course, covering Lexical Analysis (using **Flex / Lex**) and Syntax Analysis / Parsing (using **Bison / Yacc**).

---

## 📂 Laboratory Practicals Overview

| Practical | Topics / Descriptions | Files |
| :--- | :--- | :--- |
| **Practical 1** | Lexical Analyzer: Token Recognition & Word/Line/Character Counting | [`prac1.l`](file:///d:/Compiler-Construction-Lab-main/Practical%201/prac1.l), [`prac1(2).l`](file:///d:/Compiler-Construction-Lab-main/Practical%201/prac1(2).l) |
| **Practical 2** | Identification of Capital Words / Identifier Filtering | [`prac2.l`](file:///d:/Compiler-Construction-Lab-main/Practical%202/prac2.l) |
| **Practical 3** | Identification of Valid Numbers (Integers & Floating-Point) | [`prac3.l`](file:///d:/Compiler-Construction-Lab-main/Practical%203/prac3.l) |
| **Practical 4** | Lex & Yacc Calculator / Expression Grammar Evaluator | [`prac4.l`](file:///d:/Compiler-Construction-Lab-main/Practical%204/prac4.l), [`prac4.y`](file:///d:/Compiler-Construction-Lab-main/Practical%204/prac4.y) |
| **Practical 5** | Recognizing Keywords, Identifiers, and Special Characters in C | [`prac5.l`](file:///d:/Compiler-Construction-Lab-main/Practical%205/prac5.l) |
| **Practical 6** | Checking Validity of Identifiers / Variable Names | [`prac6.l`](file:///d:/Compiler-Construction-Lab-main/Practical%206/prac6.l) |
| **Practical 7** | Identifying Relational and Arithmetic Operators | [`prac7.l`](file:///d:/Compiler-Construction-Lab-main/Practical%207/prac7.l) |
| **Practical 8** | Syntax Validation for Arithmetic Expressions using Yacc | [`prac8.l`](file:///d:/Compiler-Construction-Lab-main/Practical%208/prac8.l), [`prac8.y`](file:///d:/Compiler-Construction-Lab-main/Practical%208/prac8.y) |
| **Practical 9** | Syntax Validation for Conditional Statements / Infix-to-Postfix Parser | [`prac9.l`](file:///d:/Compiler-Construction-Lab-main/Practical%209/prac9.l), [`prac9.y`](file:///d:/Compiler-Construction-Lab-main/Practical%209/prac9.y) |
| **Practical 10** | Syntax-Directed Translation / Desktop Calculator with Yacc | [`prac10.l`](file:///d:/Compiler-Construction-Lab-main/Practical%2010/prac10.l), [`prac10.y`](file:///d:/Compiler-Construction-Lab-main/Practical%2010/prac10.y) |

---

## 🛠️ Prerequisites & Tools

- **Flex** (Fast Lexical Analyzer Generator)
- **Bison** (GNU Parser Generator / Yacc equivalent)
- **GCC / Clang** (C Compiler)

### On Linux (Ubuntu / Debian):
```bash
sudo apt update
sudo apt install flex bison build-essential
```

### On Windows (via MSYS2 or MinGW):
```bash
pacman -S mingw-w64-x86_64-flex mingw-w64-x86_64-bison mingw-w64-x86_64-gcc
```

---

## 🚀 How to Compile & Run

### 1. Flex Programs (e.g., Practical 1 - 3, 5 - 7):
```bash
cd "Practical 1"
flex prac1.l
gcc lex.yy.c -o prac1 -lfl
./prac1
```

### 2. Combined Flex & Bison Programs (e.g., Practical 4, 8, 9, 10):
```bash
cd "Practical 10"
bison -d prac10.y
flex prac10.l
gcc lex.yy.c prac10.tab.c -o prac10 -lm
./prac10
```

---

## 👤 Author
- **Ayush Aswale** ([@Ayush-Aswale](https://github.com/Ayush-Aswale))
