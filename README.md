# HFT-Simulator

A modular, audit-ready **High-Frequency Trading (HFT) Simulator** designed for research, recruiter/panel demos, and secure backend validation.  
This project integrates **C++ latency-critical engines**, **Python strategy prototyping**, and **Jupyter-based research notebooks** into a single reproducible workflow.

---

## 🚀 Features

- **C++ Engine (`cpp_engine/`)**
  - Ultra-low latency order book and matching engine.
  - Modular design with clear separation of concerns.
  - Audit logs and rate-limiting for demo stability.

- **Data Feed (`data_feed/`)**
  - Live Binance tick integration.
  - Synthetic signal injection for guaranteed trade history.
  - Rolling metrics and CSV logging for reproducibility.

- **Python Strategies (`python_strategies/`)**
  - LSTM and RL-based trading strategies.
  - Hybrid outputs (binary + probabilistic).
  - Automated benchmarking with instant reporting.

- **Dashboard (`dashboard/`)**
  - Real-time equity curve visualization.
  - Action distribution plots for recruiter/panel demos.
  - Demo-friendly safeguards (batch processing, throttled output).

- **Notebooks (`notebooks/`)**
  - Publication-quality charts and tables.
  - Research-ready scaffolds for appendices.
  - Automated labeling and threshold testing.

---

## 📂 Project Structure

```
HFT-Simulator/
├── cpp_engine/          # Core C++ matching engine
├── data_feed/           # Live + synthetic tick data
├── python_strategies/   # ML/RL trading strategies
├── dashboard/           # Visualization + demo outputs
├── notebooks/           # Jupyter research workflows
├── integration/         # Backend/frontend integration
├── docs/                # Documentation
├── make_labels.py       # Automated label generation
├── requirements.txt     # Python dependencies
├── environment.yml      # Conda environment
└── LICENSE              # MIT License
```

---

## ⚙️ Installation

### Prerequisites
- **C++17** or higher
- **Python 3.9+**
- **Conda** (recommended for environment management)

### Setup
```bash
# Clone repository
git clone https://github.com/MegarusherSamarth/HFT-Simulator.git
cd HFT-Simulator

# Create environment
conda env create -f environment.yml
conda activate hft-sim

# Install Python dependencies
pip install -r requirements.txt
```

---

## ▶️ Usage

### Run C++ Engine
```bash
cd cpp_engine
mkdir build && cd build
cmake ..
make
./hft_engine_demo
```

### Visualize Dashboard
```bash
python dashboard/app.py
```

### Research Notebook
Open Jupyter Lab:
```bash
jupyter lab notebooks/
```

---

## 📊 Demo Outputs

- **Equity Curve**: Plotted once at end of run for clarity.  
- **Action Distribution**: Histogram of buy/sell/hold decisions.  
- **Audit Logs**: CSV + console logs for reproducibility.  

---

## 🧪 Validation

- Rolling metrics confirm backend stability.  
- Rate-limiting ensures demo safety.  
- CSV logging supports recruiter/panel review and research appendices.  

---

## 📜 License

This project is licensed under the **MIT License**. See `[Looks like the result wasn't safe to show. Let's switch things up and try something else!]` for details.

---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you’d like to add.  
Ensure that auditability and demo-readiness are preserved in all contributions.

---

## 📧 Contact

Created by **Vaibhavi Ghildiyal**  
For collaboration or research inquiries, please reach out via GitHub.
