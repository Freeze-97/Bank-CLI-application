# Bank CLI Application in C++

This is a simple command-line based banking application written in C++. It allows users to create and manage different types of bank accounts, such as savings accounts, long-term savings accounts, and transaction accounts. The project uses object-oriented programming principles, including inheritance and polymorphism.

## Project Structure

- `main.cpp` — Entry point  
- `testProgram.h` / `testProgram.cpp` — Program to test all classes and provide menu  
- `bank.h` / `bank.cpp` — Core bank functionality  
- `konto.h` / `konto.cpp` — Base account class (Konto)  
- `bankKund.h` / `bankKund.cpp` — Bank customer class  
- `transactionAccount.h` / `transactionAccount.cpp` — Transaction account (inherits Konto)  
- `savingsAccount.h` / `savingsAccount.cpp` — Savings account (inherits Konto)  
- `longSavingsAccount.h` / `longSavingsAccount.cpp` — Long-term savings account (inherits Konto)

## Features

- Create bank customers
- Open different types of accounts
  - Transaction account
  - Savings account
  - Long-term savings account
-  Deposit and withdraw funds
- Display account information
- Test mode with predefined operations

### Compile:

```bash
g++ -std=c++17 -o bankApp main.cpp bank.cpp bankKund.cpp konto.cpp savingsAccount.cpp longSavingsAccount.cpp transactionAccount.cpp testProgram.cpp
```

### Run:

```bash
./bankApp
```
