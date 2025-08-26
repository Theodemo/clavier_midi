# 🎹 Analog Synthesizer Project – 2020/2021

## 📌 Description

This electronics project aims to design and build an **analog synthesizer**.
The system is based on:

* a **MIDI keyboard** generating digital frames,
* a **MIDI-to-analog converter (MCV4)**,
* and a **Voltage-Controlled Oscillator (VCO)** generating a triangular waveform.

The system must produce an analog signal whose **frequency matches the note played on the keyboard**.

---

## 🎯 Learning Objectives

* Apply electronics knowledge acquired during the semester.
* Dimension a system to meet a set of specifications.
* Study a system as a black box and characterize it experimentally.
* Assemble a circuit on a breadboard.
* Troubleshoot and characterize an electronic circuit.
* Read and understand technical documentation (keyboard, MCV4, Op-Amps, etc.).
* Write a **comprehensive technical report**.

---

## ⚙️ Project Specifications

### Output Signal

The generated signal must be:

* **triangular**, symmetric, with zero average value,
* **10 V peak-to-peak amplitude**,
* **frequency f** (f = 1/T with T = T1+T2) corresponding to the note played on the MIDI keyboard.

### Voltage-Controlled Oscillator (VCO)

* 3 main functional blocks:

  1. Generate a voltage representing the note played,
  2. Generate a ramp signal,
  3. Compare voltages to produce a triangular waveform.
* Fixed component values:

  * **C = 15 nF**
  * **R3 = 82 kΩ**
  * **Operational Amplifiers: TL081**, powered with ±13 V.
* Other resistor values must be determined to meet the specifications.

---

## 🧰 Hardware & Resources

* MIDI keyboard (producing MIDI frames).
* **MCV4 converter** (Volt/Hz mode recommended).
* Breadboard + passive components (resistors, capacitors).
* **TL081 operational amplifiers**.
* Oscilloscope and ±13 V power supply.

---

## 📅 Project Timeline

* **Semester 1 (S1):** Design and implementation of the **VCO** → correct frequency generation.
* **Semester 2 (S2):** Development of the **signal envelope** to approach the sound of a real instrument.

---

## ✍️ Authors

Project carried out as part of the **Electronics – 1st year (2020/2021)** course.


