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

### 3. Block Diagram

```text
+------------------+
|    555 TIMER     |
| Clock Generator  |
+------------------+
        |
        v
+------------------+
| Seconds Counter  |
+------------------+
        |
        v
...
        |
        v
      Buzzer
```

## 4. Working Principle

### 4.1 Clock Pulse Generation

The NE555 timer is configured to generate periodic clock pulses. These pulses provide the timing signal required for the digital clock.

4.2 Seconds Counting

The clock pulses are applied to the seconds counter. The counter increments with every clock pulse and resets after reaching its maximum count.

4.3 Minutes Counting

When the seconds counter completes one full cycle, it generates a carry pulse. This carry pulse increments the minutes counter.

4.4 Hours Counting

Similarly, when the minutes counter completes one full cycle, a carry pulse is generated to increment the hours counter.

4.5 Display Section

The outputs of the counters are connected to display driver circuits. The display drivers convert the counter outputs into signals suitable for driving the 7-segment displays.

4.6 Alarm Section

The alarm time is set using switches or input controls. Logic circuitry compares the current time with the preset alarm time.

When both times match, the alarm output activates the buzzer.

5. Circuit Modules

The complete system can be divided into the following modules:

Clock Pulse Generator
Seconds Counter
Minutes Counter
Hours Counter
Display Driver
7-Segment Display
Alarm Setting Circuit
Time Comparison Logic
Buzzer / Alarm Output

6. Signal Flow
555 Timer
   |
   v
Seconds Counter
   |
   v
Minutes Counter
   |
   v
Hours Counter
   |
   v
Display Driver
   |
   v
7-Segment Display

7. Alarm Operation
Current Time --------+
                     |
                     v
              Time Comparator
                     |
                     v
Preset Alarm --------+

                  Match?
                 /      \
               Yes       No
                |         |
                v         v
              Buzzer   Continue
                        Clock


8. Output

The circuit continuously displays the current time using 7-segment displays.

When the current time matches the preset alarm time, the buzzer is activated to provide an alarm indication.

9. Conclusion

The digital clock with alarm demonstrates the practical use of the NE555 timer, digital counters, logic circuits and 7-segment displays. The project combines analog timing generation with digital counting and display techniques to implement a complete digital clock system.
