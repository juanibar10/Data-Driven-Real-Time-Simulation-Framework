# Data-Driven Real-Time Simulation Framework

A modular, scalable, **data-driven framework for real-time simulation** built with **Unity**, designed to decouple simulation logic from presentation, enable runtime observability, and support complex agent-based systems.

---

## 🎯 Purpose

This framework aims to solve a common problem in real-time simulations:

> Simulation logic tightly coupled to Unity components, hard to scale, hard to debug, and hard to reason about.

The goal is to provide:
- A **clean separation** between simulation core and Unity layer
- **Data-driven definitions** for agents and systems
- **Deterministic and testable simulation logic**
- **Runtime inspection and observability**
- A solid base for **traffic, training, and large-scale simulations**

---

## 🧠 Core Concepts

- **Data-Driven Architecture**  
  Simulation behavior is defined through data, not hardcoded MonoBehaviours.

- **Decoupled Simulation Core**  
  The simulation can evolve independently of Unity’s GameObject lifecycle.

- **Real-Time Execution**  
  Designed for real-time constraints while keeping the logic deterministic and inspectable.

- **Scalability-Oriented**  
  Built with performance, GC control, and large agent counts in mind.

---

## 🧩 High-Level Architecture

Unity Layer (Rendering, Input, Editor)
        --> Simulation Bridge (Adapters & Binding)
                --> Simulation Core (Pure C# / Data)


- **Unity Layer**  
  Visual representation, editor tools, and user interaction.

- **Simulation Bridge**  
  Translates Unity state into simulation data and vice versa.

- **Simulation Core**  
  Stateless or state-contained systems operating on structured data.

---

## 📂 Project Structure (Expected)

Assets/
- Simulation/
  - Core/        # Pure simulation logic
  - Systems/     # Simulation systems
  - Data/        # Data definitions
- Runtime/
  - Bridges/     # Unity -> Simulation adapters
- Editor/
  - Tools/       # Debug & visualization tools
- Samples/
  - Examples/



---

## ▶️ Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/juanibar10/Data-Driven-Real-Time-Simulation-Framework.git
