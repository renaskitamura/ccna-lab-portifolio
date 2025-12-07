# Lab 01: Connecting Devices (Layer 1)

### Objective
To practice selecting the correct cabling types for various network devices, distinguishing between Straight-through, Crossover, and Fiber Optic connections based on device roles (MDI vs MDI-X).

### Topology
![Network Topology](topologylab1.png)

### Concepts Applied
* **Copper Straight-Through:** Used for unlike devices (e.g., Switch ↔ PC, Switch ↔ Router).
* **Copper Crossover:** Used for like devices (e.g., Switch ↔ Switch, Router ↔ Router).
* **Fiber Optic:** Used for long-distance connections (R1 ↔ R3 were 3km apart, requiring Single-Mode fiber and R3 ↔ R4 were 250m apart which is too long for UTP cable, requiring fiber again but this time the Multimode will be enough since it can go up to 550m).

### My Learning Notes
In this lab, I learned that devices transmit and receive on specific pins (1 & 2 or 3 & 6).
* **PC/Routers:** Transmit on 1 & 2.
* **Switches:** Transmit on 3 & 6.
If I connect two Switches together, I must use a **Crossover cable** so the Transmit pins on one end connect to the Receive pins on the other.

### The "Chef" Perspective
In the kitchen, gas lines and water lines look similar but connecting them wrong is catastrophic. Similarly, in networking, plugging a Router into another Router with a straight-through cable (without Auto-MDIX) means the data "flow" hits a wall. Understanding the physical medium is just like understanding your ingredients. You have to know what goes where before you start cooking.

### Files included
* [Day 01 Lab - Connecting Devices](https://github.com/renaskitamura/ccna-lab-portifolio/blob/main/01-Connecting-Devices/Day%2001%20Lab%20-%20Connecting%20Devices.pkt) - The Packet Tracer source file.
