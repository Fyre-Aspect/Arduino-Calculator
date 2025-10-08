# 🧮 Arduino Numpad Calculator

This project demonstrates how to build a **fully functional calculator** using an **Arduino Uno**, a **4x4 Matrix Keypad**, and a **16x2 LCD Display**.  
It performs basic arithmetic operations — **Addition, Subtraction, Multiplication, and Division** — using physical button inputs.

---

## 📦 Components Required

| Component | Quantity | Description |
|------------|-----------|-------------|
| Arduino Uno | 1 | Main microcontroller |
| 4x4 Matrix Keypad | 1 | For number and operation input |
| 16x2 LCD Display | 1 | To show input and results |
| Jumper Wires | ~15 | For connections |
| Breadboard | 1 | Optional, for easier wiring |
| USB Cable | 1 | For uploading code |

---

## ⚙️ Step 1: Circuit Wiring

Follow the diagram below for connecting all components correctly.

> 🖼️ **Wiring Diagram:**
>
> ![Arduino Calculator Wiring](0013b4a8-d2ac-4961-920e-98e74dcb789b.png)

### 🔌 **Connections**

#### Keypad → Arduino
| Keypad Pin | Arduino Pin | Description |
|-------------|--------------|-------------|
| Row 1 | D9 | Input Row |
| Row 2 | D8 | Input Row |
| Row 3 | D7 | Input Row |
| Row 4 | D6 | Input Row |
| Col 1 | D5 | Input Column |
| Col 2 | D4 | Input Column |
| Col 3 | D3 | Input Column |
| Col 4 | D2 | Input Column |

#### LCD → Arduino (Parallel Connection)
| LCD Pin | Arduino Pin | Description |
|----------|--------------|-------------|
| RS | D12 | Register Select |
| E | D11 | Enable |
| D4 | D10 | Data 4 |
| D5 | D9 | Data 5 |
| D6 | D8 | Data 6 |
| D7 | D7 | Data 7 |
| VSS | GND | Ground |
| VDD | 5V | Power |
| RW | GND | Write Mode |
| V0 | Potentiometer | Adjust LCD Contrast |

> 💡 If using an **I2C LCD**, connect **SDA → A4** and **SCL → A5**, and remove the individual data pins.

---

## 💾 Step 2: Install Libraries

Before uploading the code, install the required Arduino libraries.

1. **Keypad Library**
   - Go to: `Sketch → Include Library → Manage Libraries...`
   - Search for **Keypad** by Mark Stanley & Alexander Brevig
   - Click **Install**

2. **LiquidCrystal Library**
   - Pre-installed with the Arduino IDE.

---

## 💻 Step 3: Upload the Code

Copy and paste the following code into your Arduino IDE:

  }
}
