# 🏦 Bank Management System (MIPS Assembly)

## 📌 Project Overview
This project is a simplified **Bank Management System** implemented using **MIPS Assembly Language**.  
It simulates core banking operations such as account registration, login authentication, balance inquiry, deposit, withdrawal, and fund transfer.

The system is designed to demonstrate low-level programming concepts including:
- Memory management
- System calls
- Control flow (branching & looping)
- String handling
- Register manipulation

---

## 🎯 Features

### 🔐 Authentication System
- User Registration
- Login with username & password
- Limited login attempts handling

### 💰 Banking Operations
- Deposit money
- Withdraw money
- Check account balance
- Fund transfer between accounts

### 👤 Account Management
- Display user information (name, address, contact)
- Secure storage of user credentials

### 🚪 System Control
- Main menu navigation
- Logout functionality
- Exit handler

---

## 🏗️ System Architecture

The system is built using MIPS `.data` and `.text` sections:

### 📦 Data Section
Stores:
- User information
- Credentials (username/password)
- Balance variable
- Messages and prompts

### ⚙️ Text Section
Contains the program logic:
- Menu system
- Authentication logic
- Banking operations
- Control flow

---

## 🔧 How It Works

1. User starts the program
2. Main menu is displayed:
   - Register
   - Login
   - Exit
3. After login:
   - Account dashboard appears
   - User can perform banking operations
4. Data is updated in memory during runtime

---

## 🧠 Key Concepts Used
- MIPS system calls (`syscall`)
- Conditional branching (`beq`, `bnez`)
- String comparison (`strcmp`)
- Memory access (`lw`, `sw`)
- Arithmetic operations (`add`, `sub`)
- Jump instructions (`j`, `jal`)

---

## 🖥️ Requirements
- MIPS simulator (QtSPIM or MARS)
- Basic understanding of assembly language

---

## 🚀 How to Run

1. Open the `.asm` file in **QtSPIM / MARS**
2. Assemble the code
3. Run the program
4. Interact using console input

---

## 📊 Project Goals
- Understand low-level system design
- Simulate real-world banking logic
- Strengthen assembly programming skills
- Practice control flow and memory handling

---

## 📌 Conclusion
This project demonstrates how a complete banking system can be simulated using MIPS assembly language. It provides hands-on experience in low-level programming and helps bridge the gap between hardware operations and software logic.

