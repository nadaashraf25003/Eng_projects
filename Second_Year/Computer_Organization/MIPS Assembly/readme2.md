# 🐍 Snake Game Project (MIPS Assembly)

## 📌 Project Overview
This project implements the classic **Snake Game** using **MIPS Assembly Language**.  
It demonstrates how low-level programming can be used to create a real-time interactive game using direct memory manipulation and bitmap display rendering.

The game includes snake movement, growth, collision detection, and apple generation using system-level operations.

---

## 🎯 Features

### 🐍 Game Mechanics
- Snake movement (up, down, left, right)
- Snake growth after eating apple
- Collision detection (walls and self-collision)

### 🍎 Apple System
- Random apple generation
- Respawn after being eaten

### 🎮 Graphics System
- Bitmap display rendering using frame buffer
- Pixel-level drawing in memory

---

## 🏗️ System Design Overview

### 🧩 Game Components
- Snake Head & Body
- Apple
- Frame Buffer (Bitmap Display)
- Input Handling (keyboard or control system)

---

## 🧠 Memory Design

### 📦 Frame Buffer
- Reserved memory: `0x80000 bytes`
- Used to render the game grid visually

### 📍 Game Variables
- `xPos`, `yPos` → Snake head position  
- `appleX`, `appleY` → Apple position  
- `xVel`, `yVel` → Snake movement direction  
- `tail` → Tracks snake tail position  

### 🔄 Conversion Constants
- `xConversion = 64` → Row width mapping  
- `yConversion = 4` → Pixel size (4 bytes per cell)

---

## ⚙️ Code Structure

The program is divided into modular sections:

### 🟢 Main Flow
- Game initialization
- Game loop execution
- Screen rendering

### 🟡 Update Functions
- `updateSnake`
- `updateSnakeHeadPosition`
- `removeTail`

### 🔵 Rendering Functions
- Draw background
- Draw border
- Draw snake
- Draw apple

### 🔴 Game Logic
- Collision detection
- Apple generation
- Movement handling

---

## 🔧 Key Concepts Used

- MIPS system calls (`syscall`)
- Stack operations (`push/pop simulation`)
- Register manipulation
- Memory addressing
- Frame buffer graphics
- 2D → 1D coordinate conversion
- Conditional branching (`beq`, `bne`)

---

## 🖥️ How It Works

1. Initialize game memory and variables  
2. Draw background and borders  
3. Place initial snake and apple  
4. Enter game loop:
   - Read input / update direction  
   - Move snake head  
   - Update tail  
   - Check collisions  
   - Refresh bitmap display  

---

## 🛠️ Requirements

- MARS MIPS Simulator  
- Bitmap Display enabled in MARS  
- Basic understanding of MIPS assembly  

---

## 🚀 How to Run

1. Open project in **MARS simulator**
2. Enable **Bitmap Display tool**
3. Connect framebuffer address
4. Assemble and run the program
5. Control snake and play the game

---

## 📊 Results
- Smooth snake movement in real time
- Proper apple generation
- Collision detection works correctly
- Frame buffer rendering successfully displays graphics

---

## 📌 Conclusion
This project demonstrates how a complete interactive game can be built using **low-level MIPS assembly language**. It strengthens understanding of computer architecture concepts such as memory management, stack operations, and graphical rendering through direct hardware-level simulation.

Despite the complexity of assembly programming, the project successfully implements a fully functional Snake game with real-time updates and graphical output.

