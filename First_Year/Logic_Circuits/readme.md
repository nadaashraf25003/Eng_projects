# 🎮 Tic Tac Toe Hardware Game

## 📖 Overview
This project implements a **Tic Tac Toe game using digital logic circuits**.  
The game is played using **push buttons as inputs** and **LEDs as outputs**, where players take turns placing their moves on a 3×3 grid.

- Player 1 → 🔴 Red LED  
- Player 2 → 🟢 Green LED  

The system ensures correct gameplay logic including **turn control, memory storage, winner detection, and draw condition**.

---

## 🎯 Objective
- Design a **3×3 Tic Tac Toe game** using hardware components  
- Prevent illegal moves (overwriting cells)  
- Detect **winner or draw conditions**  
- Maintain game state using memory elements  

---

## ⚙️ System Features
- 9 push buttons representing the grid cells  
- Dual-color LEDs for player indication  
- Turn-based player switching  
- Move locking (no overwriting allowed)  
- Reset functionality at any time  
- Automatic winner detection  
- Draw detection with LED indication  
- Game lock after win  

---

## 🧠 System Design

### 🔹 Input Layer
- 9 push buttons → represent game cells  
- Each button corresponds to one position in the grid  

---

### 🔹 Memory Unit (Flip-Flops)
- Push buttons alone cannot store state  
- **Flip-flops are used to store each move**
- Prevents data loss after releasing the button  

#### Problem Solved:
- Prevents cheating (pressing same button multiple times)  
- Ensures each cell is written only once  

---

### 🔹 Player Selector
- Uses **XOR logic** to alternate turns between players  

#### Logic:
- Odd presses → Player 1  
- Even presses → Player 2  

- Output controls LED color:
  - `1 → Red (Player 1)`
  - `0 → Green (Player 2)`

---

### 🏆 Winner Detection
There are **8 possible winning combinations** in Tic Tac Toe:
- 3 rows  
- 3 columns  
- 2 diagonals  

✔ Implemented using:
- AND gates for each winning condition  
- Separate circuits for each player  

#### Behavior:
- Once a player wins → output is locked  
- Further moves are ignored  

---

### 🤝 Draw Detection
- Occurs when:
  - All 9 cells are filled  
  - No winner is detected  

✔ Implemented using:
- AND gates to check all inputs  
- Combined with winner output  

➡ A dedicated LED indicates a draw  

---

### 🔒 Game Lock Mechanism
- Once a winner is detected:
  - Remaining buttons are disabled  
  - No further changes allowed  

✔ Achieved using AND gates controlled by winner signal  

---

### 🔄 Reset System
- A reset button clears:
  - All flip-flops  
  - Game state  
  - LEDs  

➡ Starts a new game instantly  

---

## 🔢 Counter System
- Uses **Asynchronous Counter (JK Flip-Flops)**  
- Counts button presses (0 → 9)  
- Helps manage turn switching logic  

---

## 🧪 Testing
- Verified correct player switching  
- Ensured no overwriting of moves  
- Tested all 8 winning conditions  
- Validated draw scenario  
- Checked reset functionality  

---


## 🚀 Applications
- Digital logic design learning  
- Educational electronics projects  
- FPGA / hardware implementation practice  

---

## ⚠️ Notes
- Ensure proper debouncing for push buttons  
- Use stable clock signal for flip-flops  
- Double-check wiring for correct logic operation  
