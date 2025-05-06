# Week 1 Report – ENGDRAW501: Design for Manufacturing 2025  
**Project:** Automated Pharmaceutical Pill Sorting System  
**Author:** CJ Jarmaine  
**Date:** Week 1 – 2025  
**Institution:** TAFE SA  

---

## 1. Project Overview

The goal of this capstone project is to design and develop an **automated pill sorting system** capable of identifying and separating pharmaceutical pills based on colour using **sensor-guided automation**. This system will integrate mechanical, electrical, and embedded systems engineering principles to deliver a low-cost, scalable solution suitable for pharmacy or aged-care environments.

---

## 2. Functional Requirements

- Detect pill presence and colour.
- Identify pills by RGB colour classification.
- Sort pills into correct bins using actuators.
- Handle variable pill types and sizes.
- Operate autonomously with minimal user interaction.
- Powered by a single 5V or 12V DC source (expandable to battery/solar in future).

---

## 3. Subsystems Identified

| Subsystem       | Description |
|----------------|-------------|
| **Sensing**     | Colour detection using TCS34725 I2C sensors. |
| **Control**     | Central processing using ESP32-WROOM-32 microcontroller. |
| **Power**       | Step-down converter to supply 5V/3.3V; main supply 12V. |
| **Actuation**   | Linear actuators (24V) for bin sorting. |
| **Mechanics**   | Sliding conveyor or gravity-feed channel with guide rails. |
| **Communication** | USB/serial debug; optionally Wi-Fi for OTA or logging. |

---

## 4. Week 1 Objectives

- Brainstorm system design ideas.
- Perform research on similar systems and feasible sensor-actuator combinations.
- Define project deliverables and milestones.
- Set up version control using Git for all project documentation and code.
- Establish shared folder structure for schematics, mechanical drawings, and firmware.

---

## 5. Tasks Completed

- Finalised project topic and scoped initial goals.
- Selected key components:
  - ESP32-WROOM-32
  - TCS34725 colour sensor
  - 24V DC linear actuators with relay interface
- Created Git repository and initial directory structure.
- Drafted high-level system architecture (to be digitised in Week 2).
- Confirmed use of KiCad for schematic and PCB design.

---

## 6. Initial Component Research

| Component        | Reason for Selection |
|------------------|----------------------|
| **ESP32-WROOM-32** | Dual-core MCU with Wi-Fi, ample GPIO, and sleep modes. |
| **TCS34725**       | Accurate RGB sensor with I2C interface and interrupt support. |
| **Relay Board**    | Enables ESP-safe control of high-current 24V actuators. |
| **Buck Converter** | Steps down 12V input to 5V/3.3V to power ESP and sensors. |

---

## 7. Issues / Risks Identified

- Pill types may have very similar colours — may need AI or calibration logic.
- Synchronising detection and actuation timing requires accurate control loop.
- Mechanical design must prevent pill jamming or misfeeds.
- Colour sensor must be shielded from ambient light.

---

## 8. Planned Week 2 Tasks

- Finalise mechanical design concepts (CAD sketches).
- Start system block diagram in KiCad.
- Breadboard sensor and test basic colour detection accuracy.
- Begin BOM (Bill of Materials) documentation.
- Research or test relay/actuator switching circuit.

---

## 9. Notes

All project files (drawings, code, documentation) are version-controlled using Git in a local repository (`pill-sorter-project`). A public repository may be created once hardware testing begins.

---
