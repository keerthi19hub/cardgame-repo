# 🃏 Card Game Engine — Object-Oriented Deck Engine & LIFO Card Mechanics

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=450A0A,DC2626,F87171&height=220&section=header&text=Card%20Game%20Engine&fontSize=42&fontColor=ffffff&fontAlignY=38&desc=Object-Oriented%20Deck%20Engine%20%26%20LIFO%20Card%20Mechanics&descSize=18&descAlignY=60&descAlign=50" width="100%" alt="Card Game Engine Banner" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Language-Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java" />
  <img src="https://img.shields.io/badge/Paradigm-Object--Oriented%20Programming-blue?style=for-the-badge" alt="OOP" />
  <img src="https://img.shields.io/badge/Architecture-Modular%20Class%20Design-450A0A?style=for-the-badge" alt="Architecture" />
  <img src="https://img.shields.io/badge/State-Deck%20%26%20Dealer%20Simulation-DC2626?style=for-the-badge" alt="Simulation" />
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" alt="License" />
</p>

---

## 📌 Table of Contents

- [📖 Executive Summary](#-executive-summary)
- [🎯 Project Overview & Objectives](#-project-overview--objectives)
- [✨ Key Technical Features](#-key-technical-features)
- [🏗️ Class Architecture & OOP Relationships](#️-class-architecture--oop-relationships)
- [🛠️ Tech Stack Matrix](#️-tech-stack-matrix)
- [⚙️ Compilation & Execution](#️-compilation--execution)
- [📁 Project Structure](#-project-structure)
- [👩‍💻 Author & Academic Context](#-author--academic-context)

---

## 📖 Executive Summary

The **Java Card Game Engine** is an object-oriented simulation modeling the mechanics of standard 52-card decks, dealer hand distribution, shuffling state transitions, and round score evaluation. Engineered with clear separation of domain concerns, the project encapsulates card rank and suit values, implements card distribution loops, and tracks dealer hand values through pure Java standard runtime libraries.

---

## 🎯 Project Overview & Objectives

- **Educational Purpose:** Demonstrating core Object-Oriented Design (OOD) patterns in Java: encapsulation, state mutability, array-based collection traversal, and modular interaction between game entities (`Dealer`, `Card`, and game driver `Main`).
- **Core Problem:** Simulating realistic card distribution requires stateful tracking of drawn cards to prevent duplicates while maintaining fair distribution routines across participants.

---

## ✨ Key Technical Features

- **🃏 Encapsulated Card Abstraction (`Card.java`):** Private field encapsulation of card suit, rank, and numeric face valuations with public accessor methods.
- **🎩 Stateful Dealer Dispatcher (`Dealer.java`):** Controls deck initialization, randomized shuffling routines, hand dealing, and score summation.
- **🔄 Game Loop Execution (`Main.java`):** Coordinates round flow, player turn simulation, console status logging, and final round determination.
- **📸 Visual Architecture Documentation:** Includes visual capture `Card game.jpg` diagramming class relationships and console execution.

---

## 🏗️ Class Architecture & OOP Relationships

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                       Card Game Class Architecture                          │
└─────────────────────────────────────────────────────────────────────────────┘
                                       │
                                       ▼
                              ┌──────────────────┐
                              │    Main.java     │  (Driver / Controller)
                              └────────┬─────────┘
                                       │
                                       ▼
                              ┌──────────────────┐
                              │   Dealer.java    │  (Deck Coordinator)
                              │  - deck: Card[]  │
                              │  - dealHand()    │
                              └────────┬─────────┘
                                       │
                                       ▼ 1..52
                              ┌──────────────────┐
                              │    Card.java     │  (Domain Entity)
                              │  - suit: String  │
                              │  - value: int    │
                              │  - rank: String  │
                              └──────────────────┘
```

---

## 🛠️ Tech Stack Matrix

| Domain | Technology | Implementation Role |
| :--- | :--- | :--- |
| **Language** | Java (JDK 8 / 11 / 17 / 21+) | Primary object-oriented programming language |
| **Compiler** | `javac` | Bytecode generation |
| **Runtime** | Java Virtual Machine (JVM) | Execution of compiled `.class` binaries |
| **Paradigm** | OOP (Encapsulation, Delegation) | Clean architectural decoupling of game entities |

---

## ⚙️ Compilation & Execution

### Prerequisites
- Java Development Kit (JDK 8 or higher) installed and configured on your `PATH`.

### 1. Clone the Repository
```bash
git clone https://github.com/keerthi19hub/cardgame-repo.git
cd cardgame-repo
```

### 2. Compile Java Source Files
```bash
javac *.java
```

### 3. Run the Game Simulation
```bash
java Main
```

---

## 📁 Project Structure

```text
cardgame-repo/
├── Card.java           # Card entity class (suit, rank, value encapsulation)
├── Dealer.java         # Deck manipulation and card dealing logic
├── Main.java           # Application entry point and game loop driver
├── Card game.jpg       # Visual documentation of execution and class design
└── README.md           # Technical documentation
```

---

## 👩‍💻 Author & Academic Context

**Keerthi N**  
- **GitHub:** [@keerthi19hub](https://github.com/keerthi19hub)  
- **Portfolio:** [keerthi19hub.github.io](https://keerthi19hub.github.io)  
- **Course:** Object-Oriented Programming in Java · Alliance University, Bengaluru  
- **Role:** Designed the card abstraction, dealer distribution loops, and round orchestration logic.

---

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=450A0A,DC2626,F87171&height=100&section=footer" width="100%" alt="Footer Banner" />
</p>
