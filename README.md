# Blink an LED – Arduino Uno

## 📌 Project Overview
The **Blink an LED** project is the classic “Hello, World!” of Arduino.  
It demonstrates how to control a digital output pin on an **Arduino Uno** to turn an LED on and off at regular intervals.

This project is perfect for beginners who want to:
- Learn the basics of Arduino programming
- Understand digital output pins
- Verify that their Arduino setup is working correctly

---

## 🧰 Components Required
- Arduino Uno
- LED
- 220Ω or 330Ω resistor
- Breadboard
- Jumper wires
- USB cable (for programming the Arduino)

---

## 🔌 Circuit Diagram (Description)
1. Connect the **long leg (anode)** of the LED to **digital pin 13** on the Arduino through a resistor.
2. Connect the **short leg (cathode)** of the LED to **GND**.
3. Plug the Arduino Uno into your computer using a USB cable.

> 💡 Note: The Arduino Uno already has a built-in LED connected to pin 13, so an external LED is optional.

---

## 💻 Arduino Code
```cpp
void setup() {
  pinMode(13, OUTPUT);
}

void loop() {
  digitalWrite(13, LOW); // Turn LED ON
  delay(1000);            // Wait 1 second
  digitalWrite(13, HIGH);  // Turn LED OFF
  delay(1000);            // Wait 1 second
}
