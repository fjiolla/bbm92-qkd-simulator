# BBM92 Quantum Key Distribution Simulator 🔐⚛️

This project implements the BBM92 quantum key distribution (QKD) protocol using Python and Qiskit. It simulates secure entanglement-based communication for satellite-to-ship scenarios in a free-space quantum channel, modeling realistic factors such as atmospheric loss, noise, and eavesdropping.

> Developed as part of a research initiative on quantum satellite-vehicular communication.

---

## 📌 Features

- ✅ BBM92 protocol with entangled qubit generation and basis reconciliation
- ✅ Atmospheric loss modeling using Beer-Lambert law
- ✅ Eavesdropper (Eve) simulation with basis mismatch and interception
- ✅ QBER (Quantum Bit Error Rate), SKR (Secret Key Rate), and throughput calculation
- ✅ SNR (Signal-to-Noise Ratio) analysis
- ✅ Comparative visualizations between **BBM92** and **MDI-QKD** (optional)
- ✅ Graphs: `QBER vs Distance`, `SKR vs Distance`, and more
- ✅ Realistic noise simulation using `qiskit_aer.noise`

---

## 🖼️ Project Architecture

<img src="diagrams/schematic_diagram.jpg" alt="System Architecture" width="500">

---

## 📊 Visualizations

### 🔷 QBER vs Distance (No Eve, No Noise)

<img src="https://github.com/fjiolla/bbm92-qkd-simulator/blob/main/diagrams/Graph1.png" alt="QBER vs Distance" width="500">

### 🔷 Secret Key Rate vs Distance

<img src="https://github.com/fjiolla/bbm92-qkd-simulator/blob/main/diagrams/graph2.png" alt="SKR vs Distance" width="500">

---

## 🧪 Installation & Setup

```bash
pip install qiskit
pip install qiskit_aer
pip install matplotlib
pip install qiskit_ibm_runtime
```

---

## ▶️ How to Run

```bash
python bbm92_simulator.py
```

Or run it in a [Google Colab notebook](https://chatgpt.com/c/684a9674-3b94-800b-abd0-39303f567fb5#) if you're using this for education/demo purposes.

---

## 🧠 What is BBM92?

The BBM92 protocol uses entangled photon pairs for secure key exchange. It is an entanglement-based variant of BB84 and is resilient against photon-number-splitting attacks.

---

## 📈 Sample Output

```
Final key length: 16
Secret key rate: 3489
Throughput: 17.892
Bit Error Rate: 0.029
Total QBER: 0.042
Total Atmospheric Loss: 18.231 dB
Eavesdropping detected: False
SNR: 2.942
```

---

## 📁 Project Structure

```
├── bbm92_simulator.py         # Core BBM92 implementation
├── diagrams/                  # Graphs and architecture diagrams
└── README.md
```

---

## 📚 Research Context

This simulator was developed as part of a research paper on **Quantum Satellite-Ship Communication using BBM92 and MDI-QKD protocols**.

---

## 🛡️ License

This project is licensed under the [MIT License](https://github.com/fjiolla/bbm92-qkd-simulator/blob/main/LICENSE).
