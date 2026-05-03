# 🧠 Web-Based Dynamic Pathfinding Agent (Wumpus World)

## 📌 Project Overview

This project implements a **Web-based Dynamic Pathfinding Agent** inspired by the **Wumpus World problem** from Artificial Intelligence.

The agent acts as a **Knowledge-Based Agent**, navigating a grid environment while:

* Receiving **dynamic percepts** (Breeze, Stench)
* Maintaining a **Propositional Logic Knowledge Base (KB)**
* Making decisions using **logical inference**

---

## 🎯 Objective

To develop an intelligent agent that:

* Safely explores an unknown environment
* Uses **logical reasoning** to deduce safe cells
* Avoids hazards like **Pits** and the **Wumpus**

---

## 🗺️ Environment Features

### ✅ Dynamic Grid

* User-defined grid size (Rows × Columns)

### ⚠️ Hazards

* Random placement of:

  * 🕳️ Pits
  * 👹 Wumpus
* Agent has **no prior knowledge** of hazard locations

### 👁️ Percepts

* **Breeze** → Adjacent to a Pit
* **Stench** → Adjacent to the Wumpus

---

## 🧠 Knowledge-Based Agent

### 📚 Knowledge Base (KB)

The agent stores logical rules such as:

B(x, y) ⇔ P(adjacent cells)
S(x, y) ⇔ W(adjacent cells)

---

### 🔍 Inference Engine

The agent uses:

* **Propositional Logic**
* **Resolution Refutation Algorithm**

Steps:

1. Convert KB into **CNF (Conjunctive Normal Form)**
2. Negate the query (e.g., "cell is safe")
3. Apply **resolution** to derive contradiction
4. Conclude if a cell is safe or dangerous

---

## 🎮 Visualization (Web UI)

### Grid Representation

* 🟩 **Green** → Safe cells
* ⬜ **Gray** → Unknown cells
* 🟥 **Red** → Hazard cells
* 🔵 **Blue** → Agent

---

## 📊 Metrics Dashboard

Displays:

* 🔢 Number of **Inference Steps**
* 👁️ Current **Percepts** (Breeze / Stench)

---

## 🛠️ Technologies Used

* HTML5
* CSS3
* JavaScript (Vanilla JS)

---

## 🚀 How to Run the Project

1. Download or clone the repository:

   ```bash
   git clone https://github.com/your-username/wumpus-agent.git
   ```

2. Open the project folder

3. Run the project:

   * Open `index.html` in your browser

---

## 🧪 How It Works

1. User selects grid size
2. Environment initializes with random hazards
3. Agent starts at (0,0)
4. Agent:

   * Receives percepts
   * Updates KB
   * Uses inference to choose next move
5. Visualization updates in real-time

---

## ⚠️ Current Limitations

* Basic inference implemented (rule-based)
* Full CNF + Resolution engine can be further improved
* No backtracking strategy yet

---

## 🔮 Future Improvements

* ✅ Full CNF conversion + resolution engine
* ✅ React-based UI
* ✅ Smarter pathfinding (A*, BFS integration)
* ✅ Probability-based reasoning
* ✅ User-controlled simulation mode

---

## 📚 AI Concepts Used

* Knowledge-Based Agents
* Propositional Logic
* Inference (Resolution Refutation)
* Wumpus World

---

## 👨‍💻 Author

**Your Name**
(Replace with your actual name)

---

## ⭐ Acknowledgment

This project is inspired by the **Wumpus World problem** from Artificial Intelligence and is developed for academic purposes.

---

## 📌 License

This project is open-source and free to use for educational purposes.
