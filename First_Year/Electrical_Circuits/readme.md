# 🔌 Power Supply for Operational Amplifiers

## 📖 Overview
This project demonstrates the design and implementation of a **regulated power supply** for operational amplifier (Op-Amp) applications.

The system converts AC input into stable DC outputs, providing:
- Adjustable positive voltage (+V)
- Adjustable negative voltage (−V)
- Fixed +5V output

It ensures **low ripple, stable voltage, and reliable performance** for analog and electronic circuits.


---

## ⚙️ Features
- Dual power supply (+V / −V)
- Adjustable output using potentiometers
- Fixed +5V output (LM7805)
- Ripple filtering using capacitors
- LED indicators for power status
- Suitable for Op-Amp and analog circuits

---

## 🧩 Components

| Component | Specification |
|----------|-------------|
| Transformer | 24-0-24V, 2A (Center-tapped) |
| Bridge Rectifier | Full-wave |
| LM317 | Adjustable positive regulator |
| LM337 | Adjustable negative regulator |
| LM7805 | Fixed +5V regulator |
| Resistors | 270Ω, 1kΩ |
| Diodes | 1N4007 |
| Capacitors | 2200µF (Electrolytic), 0.1µF (Ceramic) |
| Potentiometers | 5kΩ |
| LEDs | Green, Red |
| Switches | SPST, DPDT |

---

## ⚡ Working Principle

The system operates through four main stages:

### 1. Transformation
A center-tapped transformer steps down the AC voltage (220V → 24-0-24V).

### 2. Rectification
A bridge rectifier converts AC into pulsating DC.

### 3. Filtering
Capacitors smooth the signal by reducing ripple.

### 4. Regulation
- LM317 → Adjustable +V  
- LM337 → Adjustable −V  
- LM7805 → Fixed +5V  

---

## 🔌 Outputs
- Adjustable positive voltage (+V)
- Adjustable negative voltage (−V)
- Fixed +5V output

---

## 🧪 Testing
- Verified voltage stability
- Measured ripple reduction
- Tested regulator performance
- Checked LED indicators

---

## 📷 Project Preview

### 🔧 Schematic
![Schematic](images/schematic.png)

### 🧱 Final Design
![Final Design](images/final_design.png)

---

## 🚀 Applications
- Operational amplifier circuits
- Analog electronics labs
- Embedded systems
- Educational projects

---

## ⚠️ Safety Notes
- Use heat sinks with voltage regulators
- Check polarity before powering the circuit
- Ensure proper insulation and connections

---

## 📜 License
This project is for educational purposes.
