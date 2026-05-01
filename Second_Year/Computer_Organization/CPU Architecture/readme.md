# 🧠 32-bit Single-Cycle Processor (CPU Architecture)

## 📖 Overview
This project focuses on the **design and simulation of a 32-bit single-cycle processor** capable of executing a minimal instruction set.

The processor supports:
- Arithmetic operations  
- Logical operations  
- Conditional branching  
- Jump instructions  

All instructions are executed in **one clock cycle**, making the design simple and suitable for educational purposes.

---

## 👥 Team Members
- Gehad Amr  
- Eslam Ahmed  
- Nada Ashraf  
- Nesreen Ahmed  
- Nour Abd El-Sater  

**Supervisor:**  
Dr. Lamia Alrefaai  

---

## 🎯 Project Goal
To design and simulate a CPU that:
- Executes instructions in a single cycle  
- Demonstrates datapath and control unit interaction  
- Supports a basic instruction set architecture (ISA)  

---

## ⚙️ CPU Architecture Overview

The processor consists of the following main components:

- Program Counter (PC)  
- Instruction Memory  
- Control Unit  
- Register File (32 registers × 32-bit)  
- ALU (Arithmetic Logic Unit)  
- Data Memory  
- Sign Extend Unit  
- Adders  
- Multiplexers (MUX)  

---

## 🧠 What is a Single-Cycle Processor?

A **single-cycle processor** executes each instruction in one clock cycle, including:
1. Instruction Fetch  
2. Instruction Decode  
3. Execute  
4. Memory Access  
5. Write Back  

✔ Simple design  
❌ Long clock cycle (limited by slowest instruction)

---

## 🔧 Component Description

### 🔹 Program Counter (PC)
- Holds address of current instruction  
- Increments by 4 or changes for branch/jump  

---

### 🔹 Instruction Memory
- Stores program instructions  
- Outputs 32-bit instruction  

---

### 🔹 Control Unit
- Decodes opcode  
- Generates control signals:
  - RegDst, ALUSrc, MemtoReg  
  - RegWrite, MemRead, MemWrite  
  - Branch, Jump, ALUOp  

---

### 🔹 Register File
- 32 general-purpose registers  
- Reads two operands and writes one result  

---

### 🔹 ALU
- Performs arithmetic and logic operations  
- Outputs result + Zero flag  

---

### 🔹 ALU Control
- Determines exact ALU operation  
- Uses ALUOp + funct field  

---

### 🔹 Data Memory
- Used in:
  - `LW` → read  
  - `SW` → write  

---

### 🔹 Adders
- PC + 4 → next instruction  
- Branch address calculation  

---

### 🔹 Shift Left 2
- Aligns branch offset (×4)  

---

### 🔹 Multiplexers (MUX)
- Control data flow:
  - ALUSrc → register / immediate  
  - RegDst → rd / rt  
  - MemtoReg → ALU / memory  
  - PCSrc → sequential / branch  

---

### 🔹 Branch Logic (BEQ & BNE)
- Uses Zero flag:
  - BEQ → branch if Zero = 1  
  - BNE → branch if Zero = 0  

---

## 🔁 Supported Instructions

### 🔢 Arithmetic
- `ADD rd, rs, rt`
- `SUB rd, rs, rt`
- `SLT rd, rs, rt`

---

### 🔗 Logic
- `AND rd, rs, rt`
- `OR rd, rs, rt`
- `NOR rd, rs, rt`
- `NAND rd, rs, rt` *(custom)*

---

### 💾 Memory
- `LW rt, offset(rs)`
- `SW rt, offset(rs)`

---

### 🔀 Branch
- `BEQ rs, rt, offset`
- `BNE rs, rt, offset`

---

### 🚀 Jump
- `JUMP address`

---

## 🔄 Instruction Execution Example (ADD)

Steps:
1. Fetch instruction from memory  
2. Decode instruction  
3. Read registers rs and rt  
4. ALU performs addition  
5. Result written to rd  

---

## 🧪 Simulation
- Implemented and tested using digital simulation tools  
- Verified:
  - Arithmetic correctness  
  - Branching behavior  
  - Memory operations  

---

## 📌 Conclusion
The single-cycle processor provides a clear understanding of how instructions are executed inside a CPU.  

Although it has performance limitations, it is an essential foundation for learning advanced architectures like:
- Multi-cycle processors  
- Pipelined processors  

