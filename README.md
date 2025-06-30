# mini-js-interpreter

MiniJS is a lightweight interpreter written in C that supports a subset of JavaScript-like syntax. It was built as a learning project to understand how lexers, parsers, and interpreters work together to process and execute code.

---

## Features
✅ **Variable Declarations**
- `let`, `var`, `const` keywords  
- Enforces `const` immutability

✅ **Arithmetic Expressions**
- Supports `+`, `-`, `*`, `/` operators
- Supports parentheses for grouping

✅ **Assignments**
- Reassign variables (`let` and `var`)  
- Error on assigning to `const`

✅ **Print Statements**
- `print()` function to display results

✅ **Error Handling**
- Undefined variables
- Redeclarations
- Division by zero

---

## Project Structure
├── main.c # Entry point
├── lexer.c / lexer.h # Tokenizer (lexer)
├── parser.c / parser.h # Recursive descent parser and evaluator
├── interpreter.c / interpreter.h # Symbol table and execution logic

## Build Instructions
Compile with GCC:

```bash
gcc -o minijs main.c lexer.c parser.c interpreter.c
