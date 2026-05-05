# Cornell Notes

## Topic: Scope Rules

## Date: 05/05/2026

---

### Cue Column (Questions, Keywords, or Prompts)

- [Insert question or keyword]
- [Insert question or keyword]
- [Insert question or keyword]

---

### Notes Section (Main Notes)

#### Scope Rules
- C++ uses scope rules to determine where an identiﬁer can be used
- C++ uses static or lexical scoping
- Local or Block scope
- Global scope

#### Local or Block Scope
- Identiﬁers declared in a block { }
- Function parameters have block scope
- Only visible within the block { } where declared
- Function local variables are only active while the function is executing
- Local variables are NOT preserved between function calls
- With nested blocks inner blocks can ‘see’ but outer blocks cannot ‘see’ in

#### Static local variables
- Declared with static qualiﬁer 
```cpp
static int value {10};
```
- Value IS preserved between function calls
- Only initialized the ﬁrst time the function is called

#### Global scope
- Identiﬁer declared outside any function or class
- Visible to all parts of the program after the global identiﬁer has been declared
- Global constants are OK
- Best practice – don’t use global variables

#### How do Function Calls Work?
- **Functions use the `function call stack`**
  - Analogous to a stack of books
  - LIFO – Last In First Out
  - push and pop
- **Stack Frame or Activation Record**
  - Functions must return control to function that called it
  - Each time a function is called we create an new activation record and push it on stack
  - When a function terminates we pop the activation record and return
  - Local variables and function parameters are allocated on the stack
- Stack size is ﬁnite – Stack Overﬂow


---

### Summary Section (Summary of Notes)

[Insert a brief summary of the key ideas and takeaways]