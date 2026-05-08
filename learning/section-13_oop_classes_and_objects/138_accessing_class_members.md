# Cornell Notes

## Topic: Accessing Class Members

## Date: 08/05/2026

---

### Cue Column (Questions, Keywords, or Prompts)

- How do you access class members in C++?
- What is the difference between public, private, and protected members?
- How do you use getter and setter methods?

---

### Notes Section (Main Notes)

#### Accessing Class Members
- We can access
    - class attributes
    - class methods
- Some class members will not be accessible (more on that later)
- We need an object to access instance variables
- If we have an object (dot operator)
- Using the dot operator
```cpp
Account frank_account;
frank_account.balance;
frank_account.deposit(1000.00);
```
- If we have a pointer to an object (member of pointer operator)
- Dereference the pointer then use the dot operator.
```cpp
Account
*frank_account = new Account();
(*frank_account).balance;
(*frank_account).deposit(1000.00);
```
- Or use the member of pointer operator (arrow operator)
```cpp
Account *frank_account = new Account();
frank_account->balance;
frank_account->deposit(1000.00);
```
#### Class Member Access Modiﬁers

- `public`, `private`, and `protected`
- `public`
  - accessible everywhere
```cpp
class Class_Name
{
    public:
    // declaration(s);
};
```

- `private`
  - accessible only by members or friends of the class
```cpp
class Class_Name
{
private:
// declaration(s);
};
```

- `protected`
  - used with inheritance – we’ll talk about it in the next section
```cpp
class Class_Name
{
    protected:
    // declaration(s);
};
```


---

### Summary Section (Summary of Notes)

[Insert a brief summary of the key ideas and takeaways]