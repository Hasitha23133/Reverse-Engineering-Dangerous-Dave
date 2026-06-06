# Reverse-Engineering-Dangerous-Dave
Reverse Engineering and Runtime Manipulation Analysis of the Dangerous Dave DOS Game using DOSBox-X Debugger for the SLIIT Software Secure Systems (IE3042) Module.

# 🎮 Reverse Engineering and Runtime Manipulation of Legacy Game Software

![License](https://img.shields.io/badge/License-MIT-green.svg)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 📌 Project Overview

This project was completed for the **Software Secure Systems (IE3042)** module at SLIIT.

The objective was to analyze a legacy DOS game using reverse engineering techniques, identify runtime memory locations, trace assembly-level instructions, and evaluate security weaknesses that allow runtime manipulation.

The selected game was **Dangerous Dave (DOS Version)**.

---

## 🎯 Objectives

* Perform reverse engineering on a legacy game.
* Analyze runtime memory behavior.
* Identify life-related memory variables.
* Trace assembly instructions that access game state.
* Demonstrate runtime manipulation.
* Evaluate security weaknesses.
* Recommend mitigation techniques.

---

## 🎮 Selected Game

**Dangerous Dave (DOS Version)**

Reasons for selection:

* Legacy DOS application
* Simple runtime architecture
* No modern anti-debugging protections
* Predictable memory layout

---

## 🛠️ Tools Used

* Windows Operating System
* DOSBox-X
* DOSBox-X Debugger
* Dangerous Dave Game Executable

---

## 🔍 Analysis Summary

### Static Analysis

Observed assembly instructions:

* MOV
* CMP
* JNE
* Runtime branching instructions

### Dynamic Analysis

The game life counter was monitored during gameplay and memory values were tracked after player death events.

### Memory Identification

Identified life-related memory address:

```assembly
2D70:56EE
```

### Assembly Analysis

Observed code block:

```assembly
mov ax,[56EE]
cmp ax,FFFF
jne 00001462
```

---

## 🔒 Security Findings

Missing protections:

* No Anti-Debugging
* No Memory Protection
* No Integrity Validation
* No Code Obfuscation
* Predictable Memory Layout

---

## 🛡️ Recommended Mitigations

* Anti-Debugging Techniques
* Integrity Verification
* Memory Protection
* Code Obfuscation
* Randomized Memory Layout
* Runtime Validation Checks

---

## 📸 Screenshots

Add screenshots from:

* DOSBox Startup
* Dangerous Dave Game
* Debugger Window
* Memory Search Results
* Assembly Code View
* Runtime Manipulation Evidence

---

## 📄 Project Report

[View Full Report](./SSS%20-%20IT23659230.pdf)

---

## 👨‍🎓 Author

Lakshan W M H C

IT23659230

Sri Lanka Institute of Information Technology (SLIIT)

---

## 📄 License

MIT License
