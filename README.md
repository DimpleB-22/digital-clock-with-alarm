# Digital Clock with Alarm

## 📖 Project Overview

This project implements a **Digital Clock with Alarm** using discrete electronic components. The system generates clock pulses, counts time in seconds, minutes and hours, and displays the current time using 7-segment displays.

An **NE555 timer** is used as the clock pulse generator, while digital counters and logic ICs perform the time counting and control operations. The system also includes an alarm feature that compares the current time with a preset alarm time and activates a buzzer when both values match.

---

## ✨ Features

- Real-time clock pulse generation using NE555 timer
- Seconds, minutes and hours counting
- Cascaded counter operation
- 7-segment time display
- Preset alarm functionality
- Time comparison logic
- Buzzer activation when alarm time matches
- Modular circuit design

---

## 🧩 Main Components

- NE555 Timer
- Counter ICs
- Logic ICs
- 7-Segment Display Driver ICs
- 7-Segment Displays
- Resistors
- Capacitors
- Push Buttons / Switches
- Buzzer
- Power Supply

---

## 🏗️ Block Diagram

```text
+----------------------+
|      555 TIMER       |
|   Clock Generator    |
+----------+-----------+
           |
           v
+----------------------+
|   Seconds Counter    |
+----------+-----------+
           |
           v
+----------------------+
|   Minutes Counter    |
+----------+-----------+
           |
           v
+----------------------+
|    Hours Counter     |
+----------+-----------+
           |
           v
+----------------------+
|    Display Driver    |
+----------+-----------+
           |
           v
+----------------------+
|  7-Segment Display   |
+----------------------+

Alarm Setting
      |
      v
+----------------------+
|     Alarm Logic      |
+----------+-----------+
           |
           v
        Buzzer
```

---

## ⚙️ Working Principle

### 1. Clock Pulse Generation

The NE555 timer is configured to generate periodic clock pulses. These pulses provide the timing signal required for the digital clock.

### 2. Seconds Counting

The clock pulses are applied to the seconds counter. The counter increments with every clock pulse and resets after reaching its maximum count.

### 3. Minutes Counting

When the seconds counter completes one full cycle, it generates a carry pulse. This carry pulse increments the minutes counter.

### 4. Hours Counting

Similarly, when the minutes counter completes one full cycle, a carry pulse is generated to increment the hours counter.

### 5. Display Section

The outputs of the counters are connected to display driver circuits. The display drivers convert the counter outputs into signals suitable for driving the 7-segment displays.

### 6. Alarm Section

The alarm time is set using switches or input controls. Logic circuitry compares the current time with the preset alarm time.

When both times match, the alarm output activates the buzzer.

---

## 🔔 Alarm Operation

```text
Current Time --------+
                     |
                     v
              Time Comparator
                     |
Preset Alarm --------+
                     |
                  Match?
                 /      \
               Yes       No
                |         |
                v         v
             Buzzer    Continue
                        Clock
```

When the current time matches the preset alarm time, the buzzer is activated. Otherwise, the clock continues normal operation.

---

## 📁 Repository Structure

```text
digital-clock-with-alarm/
│
├── images/
│   └── Project images and circuit diagrams
│
├── README.md
│
└── circuit-design.md
```

---

## 📄 Circuit Documentation

Detailed circuit design, block diagrams, working principle, signal flow and alarm operation are available in:

➡️ `circuit-design.md`

---

## 🚀 Future Improvements

- Add AM/PM functionality
- Add snooze functionality
- Add multiple alarm settings
- Implement automatic brightness control
- Design and simulate the complete circuit
- Implement the design using FPGA or a microcontroller

---

## 🎯 Conclusion

The Digital Clock with Alarm demonstrates the practical use of the NE555 timer, digital counters, logic circuits and 7-segment displays. The project combines analog timing generation with digital counting and display techniques to implement a complete digital clock system with alarm functionality.
