# Quasar
> Quasar will not be finished for at least 18 months, this is by far my largest and most complex project.
> **Quasar is an interactive quantum circuit simulator with a high-performance Rust/WASM core and real-time 3D visualizations.**

This project is a web-based quantum computing playground built from first principles, designed to make the fundamental concepts of quantum mechanics intuitive, interactive, and visually stunning.

## About The Project

Quantum computing is often treated as a black box, with its principles hidden behind complex mathematics and esoteric SDKs. **Quasar** aims to change that. It is an engineering and educational tool that demonstrates the core mechanics of quantum computation, built from the ground up.

The simulation engine is written in **Rust** and compiled to **WebAssembly (WASM)**, ensuring near-native performance for the complex linear algebra required. The frontend is a modern **React/TypeScript** application, providing a seamless and intuitive drag-and-drop interface for building and testing quantum circuits.

This project is not just a wrapper around an existing library; it is a demonstration of the ability to model a complex physical system in a robust, performant, and user-friendly software application.

## Core Features

  * **High-Performance Engine:** The core logic is powered by Rust/WASM, handling state vector and matrix calculations with exceptional speed directly in the browser.
  * **Interactive Circuit Builder:** A drag-and-drop interface to build, modify, and experiment with quantum circuits in real-time.
  * **3D Bloch Sphere Visualization:** An interactive 3D representation of single-qubit states, powered by `three.js`, helping to visualize concepts like superposition and phase.
  * **Real-time State Analysis:** Instantly view the resulting state vector and measurement probabilities of the multi-qubit system as you build your circuit.
  * **Noise Modeling:** (Planned) Simulate the effects of real-world quantum noise, such as decoherence and gate errors.
  * **Classic Algorithm Presets:** (Planned) Load pre-built circuits for famous algorithms like the Bell State, Quantum Teleportation, and Grover's Search.

## Technology Stack

  * **Core Engine:** [Rust](https://www.rust-lang.org/) compiled to [WebAssembly](https://webassembly.org/)
  * **Frontend:** [React](https://reactjs.org/), [TypeScript](https://www.typescriptlang.org/), [Three.js](https://threejs.org/) (for 3D graphics)
  * **Styling:** [Tailwind CSS](https://tailwindcss.com/)
  * **Testing:** [Jest](https://jestjs.io/), [React Testing Library](https://testing-library.com/docs/react-testing-library/intro/)
  * **DevOps:** [GitHub Actions](https://github.com/features/actions) for Continuous Integration (CI)

-----

## Summarised Roadmap

This project is a marathon, not a sprint. Progress is tracked in distinct, high-level phases.

  * [**In Progress**] **Phase 1: The Quantum Core**

      * [ ] Build the core simulation engine in Rust.
      * [ ] Implement complex number, vector, and matrix operations.
      * [ ] Define quantum gates (Hadamard, Pauli-X/Y/Z, CNOT).
      * [ ] Compile the Rust core to a WebAssembly module.

  * [ ] **Phase 2: The Visual Interface**

      * [ ] Set up the React/TypeScript frontend.
      * [ ] Create the static UI for the circuit grid and gate palette.
      * [ ] Implement basic state management for the circuit.

  * [ ] **Phase 3: The Connection & Visualization**

      * [ ] Integrate the WASM module with the React frontend.
      * [ ] Implement the interactive 3D Bloch Sphere visualization with `three.js`.
      * [ ] Display measurement probability bar charts.

  * [ ] **Phase 4: Advanced Simulation & Polish**

      * [ ] Implement smooth drag-and-drop functionality.
      * [ ] Add noise modeling and classic algorithm presets.
      * [ ] Write comprehensive unit and integration tests.
      * [ ] Deploy to a live URL and finalize documentation.

-----

## Getting Started

To get a local copy up and running, follow these simple steps.

### Prerequisites

  * Node.js & npm (or yarn)
  * Rust & `wasm-pack` (`cargo install wasm-pack`)

### Installation

1.  Clone the repo
    ```sh
    git clone https://github.com/YOUR_USERNAME/quasar.git
    ```
2.  Navigate to the project directory
    ```sh
    cd quasar
    ```
3.  Install NPM packages
    ```sh
    npm install
    ```
4.  Run the application
    ```sh
    npm start
    ```

## License

Distributed under the MIT License. See `LICENSE` for more information.
