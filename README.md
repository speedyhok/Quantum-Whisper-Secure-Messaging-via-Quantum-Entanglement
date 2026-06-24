# 🌌 Quantum Teleportation Messenger

A visual full-stack web application demonstrating **Quantum State Teleportation** step by step, featuring an interactive eavesdropping simulation that shows why quantum communication is physically unbreakable due to the **No-Cloning Theorem**.

Built on a **Qiskit** quantum simulator backend with a clean, glassmorphic frontend.

---

## 🧠 Core Quantum Concepts

*   **Quantum Teleportation:** Transfers the *state* (information) of a qubit to another, destroying the original in the process. It requires **2 classical bits** of helper data to reconstruct the state at the destination (meaning it cannot transmit information faster than light).
*   **No-Cloning Theorem:** Arbitrary quantum states cannot be copied. Any attempt by an eavesdropper (**Eve**) to measure or tap the quantum channel collapses the entanglement, destroying the message.
*   **Fidelity:** Measures how close the received state is to the original. A value of `1.0` (100%) represents perfect teleportation; `0.5` represents random noise (the footprint of an eavesdropper).

---

## 🛠️ Installation & Setup

1.  **Install dependencies:**
    ```bash
    pip install qiskit qiskit-aer flask numpy
    ```
2.  **Run the server:**
    ```bash
    python app.py
    ```
3.  **Access the app:** Open [http://localhost:5000](http://localhost:5000) in your browser.

---

## 🔬 How to Test

### 🟢 Safe Teleportation (No Eve)
1. Use the sliders on the left to set Adam's qubit state.
2. Click **1. Create Entangled Pair**.
3. Click **2. Measure & Send**.
4. Click **3. Apply Corrections** on Mahi's panel to rebuild the state with **100% Fidelity**.
5. Click **Run Quantum State Tomography** to statistically verify the output.

### 🔴 Intercepted Teleportation (Eve Tapping)
1. Toggle the **Eve intercepts Quantum Channel** switch.
2. Click **Create Entangled Pair** and **Measure & Send**.
3. Watch the timeline detect Eve's tap on step 2.
4. Mahi's qubit will receive random noise, dropping **Fidelity to ~50%** and triggering the security alert.

---

## 👥 Author & License

*   **Author:** **Mohibul hoque**
*   **Email:** [hokworks@gmail.com](mailto:hokworks@gmail.com)
*   **LinkedIn:** [linkedin.com/in/speedymohibul](https://www.linkedin.com/in/speedymohibul)

Distributed under the **MIT License**. See [LICENSE](LICENSE) for details.
