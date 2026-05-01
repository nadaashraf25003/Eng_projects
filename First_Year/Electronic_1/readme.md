# 🔊 Stereo Audio Amplifier

## 📖 Overview
This project presents the design and implementation of a **multi-stage stereo audio amplifier** using the **LM386 audio amplifier IC**.

The system amplifies low-power audio signals into a level sufficient to drive speakers, producing **clear and high-quality sound** suitable for small audio applications.

---

## 🎯 Project Objectives
- Design a **low-voltage stereo audio amplifier**
- Amplify weak audio signals from external sources
- Drive speakers with clear and audible sound
- Implement and test the circuit using simulation and hardware

---

## ⚙️ Features
- Stereo output (Left & Right channels)
- Based on **LM386 IC**
- Low power consumption (12V supply)
- Volume control using potentiometer
- Noise reduction using bypass capacitors
- Zobel network for output stability
- Compatible with 4Ω – 32Ω speakers

---

## 🔧 Components Used

| Component | Specification |
|----------|-------------|
| LM386 IC | Audio amplifier IC |
| Power Supply | 12V DC Adapter |
| Speakers | 8Ω |
| Resistors | 10Ω |
| Capacitors | 0.1µF (Ceramic), 100µF & 1000µF (Electrolytic) |
| Potentiometer | 50kΩ |
| LED | Green |
| Switch | SPST |
| Connectors | JST & standard connectors |

---

## 🧠 Circuit Description

The amplifier is built around the **LM386 IC**, a low-voltage audio power amplifier widely used in consumer electronics.

### 🔌 Power Supply
- Pin 6 → +12V  
- Pin 4 → Ground  

---

### 🎵 Audio Input
- Audio signal is provided via a **3.5mm jack**
- A **potentiometer (50kΩ)** is used for volume control
- A coupling capacitor removes DC components

---

### 🔇 Noise Reduction
- A **bypass capacitor (100µF)** is connected to pin 7  
- Helps reduce noise and improve signal quality  

---

### 🔊 Output Stage
- Output is taken from pin 5  
- A **1000µF capacitor** removes DC from output signal  
- Speaker (8Ω) is connected to the output  

---

### ⚖️ Zobel Network
- A resistor (10Ω) and capacitor (0.1µF) are connected in series  
- Stabilizes impedance and improves frequency response  

---

## 🧪 Experimental Testing
- Implemented on test board  
- Verified:
  - Signal amplification  
  - Sound clarity  
  - Noise levels  


---

## 📈 Results
- Clear and audible sound output  
- Stable amplification performance  
- Low noise after filtering  
- Suitable for small audio systems  

---

## ✅ Conclusion
The stereo audio amplifier successfully amplifies low-level audio signals into a usable output for speakers.  

The system demonstrates:
- Reliable performance  
- Good sound quality  
- Practical implementation for real-world applications  

---

## 📎 Attachments
- LM386 Datasheet  
- LED Datasheet  
- Capacitor Datasheets  

---

## 🚀 Applications
- Portable audio systems  
- Computer speakers  
- Educational electronics projects  
- Hobby audio amplifiers  

---

## ⚠️ Notes
- Ensure proper grounding to reduce noise  
- Use heat management if operating for long periods  
- Verify connections before powering the circuit  

