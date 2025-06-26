# Quantum Circuits Project README

This project implements five quantum computing tasks using PennyLane, designed to run in Google Colab. Each task demonstrates key quantum concepts, with circuits, measurements, and visualizations. Below is a summary of the tasks implemented.

## Task 1: Bell State Circuit
- **Description**: Creates a 2-qubit circuit to generate a Bell state, an entangled quantum state. Uses a Hadamard gate on the first qubit and a CNOT gate to entangle both qubits.
- **Features**:
  - Measures the statevector, probability distribution, and sampled outcomes.
  - Visualizes probabilities and measurement samples with plots.
  - Displays the density matrix to confirm entanglement.
  - Uses SymPy for clean matrix representation.
- **Purpose**: Demonstrates quantum entanglement and measurement outcomes for a maximally entangled state.

## Task 2: GHZ State for 3 and 4 Qubits
- **Description**: Constructs circuits for 3-qubit and 4-qubit GHZ states, which are multi-qubit entangled states. Applies a Hadamard gate to the first qubit and CNOT gates to entangle subsequent qubits.
- **Features**:
  - Measures probability distributions for all basis states.
  - Visualizes probabilities with bar plots.
  - Displays circuit diagrams using `qml.draw`.
- **Purpose**: Extends entanglement to multiple qubits, showing how GHZ states scale.

## Task 3: Rotation + Measurement Circuit
- **Description**: Builds a single-qubit circuit with an RX rotation gate, where the rotation angle is a variable input. Measures the expectation value of the Pauli-Z operator.
- **Features**:
  - Computes and plots the Pauli-Z expectation value for a range of angles (0 to 2π).
  - Visualizes the circuit using `qml.draw_mpl`.
- **Purpose**: Illustrates how a quantum state changes with rotation and how expectation values reflect this.

## Task 4: Simple Variational Optimization
- **Description**: Implements a variational quantum circuit with a single RX gate, optimizing its angle to minimize the Pauli-Z expectation value using gradient descent.
- **Features**:
  - Logs the cost (expectation value) at each optimization step.
  - Outputs the optimal angle.
  - Plots the cost function over iterations.
  - Visualizes the circuit with the optimal parameter using `qml.draw_mpl`.
- **Purpose**: Demonstrates variational quantum algorithms and optimization techniques.

## Task 5: Measurement Comparison
- **Description**: Creates a 2-qubit Bell state circuit and compares three measurement types: probabilities (`qml.probs`), samples (`qml.sample`), and expectation values (`qml.expval`).
- **Features**:
  - Prints and visualizes probabilities, sampled outcomes, and expectation values.
  - Uses separate devices for analytic (probabilities, expectation) and sampling measurements.
  - Displays the circuit using `qml.draw_mpl`.
  - Explains differences and use cases for each measurement type.
- **Purpose**: Highlights the distinct outputs of quantum measurements and their applications.

## General Notes
- **Environment**: All tasks are implemented in Python using PennyLane and are compatible with Google Colab. Dependencies (PennyLane, Matplotlib) are installed via `pip` commands.
- **Visualizations**: Tasks include plots (bar plots, histograms, or curves) and circuit diagrams using `qml.draw` or `qml.draw_mpl`.
- **Entanglement**: Tasks 1, 2, and 5 demonstrate quantum entanglement, while Tasks 3 and 4 focus on single-qubit dynamics and optimization.
- **Measurement**: Tasks explore various measurement techniques, from exact probabilities to statistical sampling, providing a comprehensive view of quantum measurement.

This project serves as an educational tool for understanding quantum circuits, entanglement, measurements, and variational algorithms in quantum computing.