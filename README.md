# The Sugar Shooter  
### Sugar High, At the Press of a Button!

**By Dayton Capson**  
**MEEN 1000**

---

## Introduction

My goal was to create a functional candy dispenser that my wife and I could enjoy in our home.  

I designed the machine to be portable and easy to use, ensuring it would be both practical and enjoyable.

### Why It Matters

Life is sweeter with chocolate! This dispenser allows us to conveniently access yummy chocolates, adding a fun and personalized touch to our home.

---

## All Components Used

### 3D Printing Materials
- Green PLA Filament
- Grey PLA Filament
- Gold PLA Filament
- Black PETG Filament
- Polymaker Polysmooth Transparent Filament

### Electronics
- Push Button
- Arduino Nano
- Small Breadboard
- 7.4v Rechargeable Wired Battery
- Main Power Switch
- Wiring
- Servo Motor

### Hardware
- Wing Nut
- Lock Nut
- Washers
- Screws
- Bearings
- Velcro

### Other Materials
- Isopropyl Alcohol (90%)
- Chocolates

---

## My Expenses

| Item                         | Cost ($) |
|------------------------------|----------|
| Green & Transparent Filament | 60.00 |
| Push Button                  | 8.99 |
| Arduino Nano                 | 11.99 |
| Breadboard                   | 8.99 |
| Batteries                    | 19.99 |
| Servo Motor                  | 14.99 |
| Hardware                     | 10.00 |
| Isopropyl Alcohol            | 5.00 |
| Chocolates                   | 20.00 |

**Estimated Total: $159.95**

---

## Post Processing – Globe

The globe is made out of **Polyvinyl Butyral (PVB)** plastic material.  
This material is commonly used in car windshields and safety glass as a bonding layer.

### Printing Settings
- Similar settings to PLA
- Print thin and slow
- 115% flow rate

### Smoothing Process
After printing, I used **90% Isopropyl Alcohol (IPA)** to smooth the layers:
- Applied 2–3 times per day
- Continued for 10 days

---

## Machine Code

*(Insert Arduino code here if you want to include it in this repository.)*

Example structure:

```cpp
// Example Servo Control Code
#include <Servo.h>

Servo myServo;
int buttonPin = 2;

void setup() {
  pinMode(buttonPin, INPUT);
  myServo.attach(9);
}

void loop() {
  if (digitalRead(buttonPin) == HIGH) {
    myServo.write(90);
    delay(500);
    myServo.write(0);
  }
}
