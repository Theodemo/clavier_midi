
# 🎹 Analog Synthesizer Project – 2020/2021

## 📌 Description

This electronics project aims to design and build an **analog synthesizer** in two phases:

* **Semester 1 (S1):** Development of a **Voltage-Controlled Oscillator (VCO)** generating a triangular waveform whose frequency corresponds to the MIDI note played.
* **Semester 2 (S2):** Design and integration of an **ADSR envelope generator** and a **multiplier (AD633)** to shape the amplitude of the signal, making the synthesizer’s output closer to a real musical instrument.

---

## 🎯 Learning Objectives

* Apply electronics knowledge acquired during the academic year.
* Dimension and design a complete system meeting given specifications.
* Study and characterize subsystems experimentally.
* Build and test circuits on breadboards.
* Troubleshoot and validate functional blocks progressively.
* Learn to use and interpret technical documentation (MIDI, MCV4, op-amps, AD633, logic circuits, etc.).
* Collaborate in teams using project management tools (Agile/Kanban).
* Write a **technical report** documenting results and methodology.

---

## ⚙️ Specifications

### Semester 1 – VCO

* **Output Signal:**

  * Triangular, symmetric, zero DC average.
  * **10 V peak-to-peak amplitude.**
  * Frequency corresponding to the note played (from MCV4 CV output).

* **Constraints:**

  * Capacitor **C = 15 nF**.
  * Resistor **R3 = 82 kΩ**.
  * **TL081 op-amps**, ±13 V supply.
  * Other resistor values to be calculated to meet requirements.

---

### Semester 2 – ADSR & Signal Shaping

* **Inputs from MCV4:**

  * **CV1 output:** Voltage proportional to frequency (Hz/V mode).
  * **GATE output:** Logic signal (0–12 V) indicating key press duration.

* **Functional Blocks:**

  * **Integrated VCO**: Provided module generating triangular waveform at note frequency.
  * **Envelope Generator (ADSR):**

    * Attack Time (AT): 100 ms (vs = 3 V at AT/2, vs = 4.2 V at AT).
    * Decay Time (DT): 100 ms (vs decreases to 3 V).
    * Sustain Level (SL): 2 V.
    * Release Time (RT): adjustable between 250–400 ms.
  * **Multiplier (AD633):** Mixes VCO triangular signal with ADSR envelope.
  * **Output Stage:** Adjustable amplification, headphone/speaker compatible.

* **Constraints:**

  * Power supplies: ±15 V for analog, +5 V regulated for digital logic (HCT family).
  * Output capacitor Cout = 0.47 µF, non-polarized.
  * GATE signal levels between 9–12 V.
  * Envelope reset must be handled.
  * Monostable circuits must be retriggerable (diode compensation required).
  * ADSR implemented using switches (HEF4066), decoder (74HCT138), and control voltages.

---

## 🧰 Hardware & Resources

* **MIDI Keyboard** (12 V powered).
* **MCV4 MIDI-to-CV Converter** (12 V powered, Hz/V mode).
* Breadboard & lab components (resistors, capacitors, switches, regulators).
* **VCO integrated module** (provided, TL082-based).
* **AD633 multiplier**.
* Oscilloscope (Tektronix, acquisition procedure provided).
* Power supplies: ±15 V and +5 V.

---

## 📅 Project Timeline

* **Semester 1 (S1):** VCO design & implementation → frequency generation.
* **Semester 2 (S2):**

  1. Design ADSR envelope generator (using logic & analog components).
  2. Integrate ADSR + VCO + AD633 multiplier.
  3. Test and validate complete synthesizer.
  4. Document simulation and real measurements (LTSpice + oscilloscope).

---

## 📑 Deliverables

* Fully wired synthesizer on lab breadboard.
* LTSpice simulation files (VCO + ADSR + complete system).
* Spreadsheet for fast recalculation of component values (based on CDC).
* Group technical report (≤ 8 pages) including:

  * Context & functional understanding.
  * Detailed characterization & proof of CDC compliance.
  * Teamwork methodology and acquired skills.

---

## ✍️ Authors

Project carried out as part of the **Electronics – 1st year (2020/2021)** course.
