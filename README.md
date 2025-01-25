# Elevator System Design Documentation

## Project Name:
Elevator System Design

## Abstract:
The project aims to design and simulate an elevator control operation circuit system using Multisim 13.0. The system incorporates five functional units: trigger latch circuit unit, code comparison circuit unit, count display circuit unit, feedback circuit unit, and delay circuit unit. These units work in tandem to simulate the operation of an elevator, including floor request handling, direction indication, and safety features like delay for door closing. The simulation demonstrates that the designed system efficiently fulfills all intended functionalities.

---

## Table of Contents:
1. **Introduction**
2. **System Overview**
3. **Circuit Design**
4. **Simulation Scenarios**
5. **Results**
6. **Conclusion**
7. **References**

---

## 1. Introduction:
The rapid development of urban infrastructure has necessitated efficient and safe vertical transportation systems like elevators. Designing and simulating elevator control circuits in software environments such as Multisim 13.0 allows for cost-effective optimization and testing of control algorithms. This project documents the design and simulation of an elevator control system with enhanced safety features and logical operations to fulfill user requests efficiently.

---

## 2. System Overview:
The elevator control system comprises five functional units:
- **Trigger Latch Circuit Unit:** Captures and latches user requests from various floors.
- **Code Comparison Circuit Unit:** Compares the current floor with the requested floor.
- **Count Display Circuit Unit:** Displays the current floor number and movement direction.
- **Feedback Circuit Unit:** Turns off the indicator for the requested floor once it is reached.
- **Delay Circuit Unit:** Extends the elevator’s stay at a floor for enhanced safety.

---

## 3. Circuit Design:

### 3.1 Trigger Latch Circuit Unit:
- **Components:** D flip-flops (74LS74D), electric switches, AND gates, indicator lights.
- **Functionality:** Captures user floor requests inside and outside the elevator. Requests are latched and displayed using D flip-flops.

### 3.2 Code Comparison Circuit Unit:
- **Components:** Comparators (74LS85D), encoders (74LS148D), logic gates.
- **Functionality:** Encodes floor requests into binary and compares the requested floor with the current floor. Generates control signals for upward, downward, or stationary operation.

### 3.3 Count Display Circuit Unit:
- **Components:** Counters (74LS192N), 7-segment LED displays, directional displays.
- **Functionality:** Updates the current floor number and indicates the direction of movement.

### 3.4 Feedback Circuit Unit:
- **Components:** Decoders (74LS139D), full adders (74LS283D), NOT gates, AND gates, OR gates.
- **Functionality:** Turns off the floor request indicator once the elevator reaches the requested floor, ensuring smooth operation.

### 3.5 Delay Circuit Unit:
- **Components:** Switches, NOT gates, high-level signal generators, indicator lights.
- **Functionality:** Delays elevator departure from a floor when required for safety.

---

## 4. Simulation Scenarios:

### 4.1 Multiple Requests with Different Directions:
- **Test Action:** Requests for floors 4 and 1 made sequentially when the elevator is at floor 2.
- **Observation:** The elevator satisfies requests sequentially, moving to floor 4 before descending to floor 1.

### 4.2 Multiple Requests in the Same Direction:
- **Test Action:** Requests for floors 2 and 1 made sequentially when the elevator is at floor 4.
- **Observation:** The elevator moves to floor 2 first, then to floor 1, satisfying requests in order.

### 4.3 Delay Function:
- **Test Action:** Request for floor 3, followed by a delay at that floor.
- **Observation:** The elevator remains at floor 3 during the delay, resuming operation once the delay is deactivated.

---

## 5. Results:
Simulation results confirm the functionality of the designed elevator control system. Key findings include:
- Accurate response to multiple user requests in the correct sequence.
- Smooth transition between floors with direction indication.
- Effective delay mechanism for enhanced safety.

---

## 6. Conclusion:
The elevator control system design successfully simulates elevator operation under various conditions. By leveraging Multisim 13.0, the system demonstrates efficient request handling, direction indication, and safety measures. Future work could focus on incorporating advanced features such as load sensors and real-time monitoring.

---

## 7. References:
- CHENG Yongmao, WEI Jiayu, LI Tianyu. “Control operation circuit system design and simulation based on Multisim 13.0.” Naval Aeronautical University, Yantai, China.
- NI Multisim 13.0 User Manual.
- IEEE Xplore Digital Library.
