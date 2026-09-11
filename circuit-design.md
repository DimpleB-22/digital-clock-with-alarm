# Circuit Design

## Project Title

### Digital Clock with Alarm Using 555 Timer, Logic ICs, Counters and 7-Segment Displays

---

## 1. Overview

This project implements a digital clock with an alarm using discrete electronic components. The circuit generates clock pulses, counts time in seconds, minutes and hours, and displays the time using 7-segment displays.

The design uses a 555 timer as the clock pulse generator along with counter, logic and display driver ICs.

---

## 2. Main Components Used

- NE555 Timer
- Counter ICs
- Logic ICs
- 7-Segment Display Driver ICs
- 7-Segment Displays
- Resistors
- Capacitors
- Push Buttons / Switches
- Buzzer for Alarm
- Power Supply

---

## 3. Block Diagram

```text
+------------------+
|    555 TIMER     |
| Clock Generator  |
+--------+---------+
         |
         v
+------------------+
| Seconds Counter  |
+--------+---------+
         |
         v
+------------------+
| Minutes Counter  |
+--------+---------+
         |
         v
+------------------+
|  Hours Counter   |
+--------+---------+
         |
         v
+------------------+
| 7-Segment Display|
+------------------+

      Alarm Setting
           |
           v
+------------------+
|   Alarm Logic    |
+--------+---------+
         |
         v
       Buzzer
