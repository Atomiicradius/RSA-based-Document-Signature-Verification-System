# 🔐 RSA-based Document Signature Verification System

> **Interactive Cryptographic Analysis and Secure Document Verification System**

A digital signature system with real-time visualization, performance analysis, and tamper detection using RSA and SHA-256.

---

## 🧠 Project Overview

This project is an **interactive digital signature and cryptographic analysis system** that:

1. Securely **signs and verifies documents** using public-key cryptography (RSA + SHA-256)
2. Visually demonstrates **how cryptographic systems behave**
3. Provides **performance analysis, attack simulation, and real-time insights**

### Key Differentiators
- 📊 Visualization of cryptographic processes
- ⚡ Performance benchmarking across key sizes
- 🎯 User-interactive security simulations
- 🔍 Avalanche effect demonstration

---

## 📁 Project Structure

```
RSA-based-Document-Signature-Verification-System/
│
├── crypto/                     # Core cryptography module (Person 1)
│   ├── __init__.py
│   ├── key_manager.py          # RSA key generation & multi-user support
│   ├── hasher.py               # SHA-256 hashing
│   ├── signer.py               # Document signing
│   └── verifier.py             # Signature verification
│
├── analysis/                   # Analysis & simulation module (Person 2)
│   ├── __init__.py
│   ├── performance.py          # Performance tracking & benchmarking
│   ├── attack_simulation.py    # File tampering & attack demos
│   ├── avalanche.py            # Avalanche effect visualization
│   └── secure_transfer.py     # Sender → Receiver simulation
│
├── ui/                         # UI & integration module (Person 3)
│   ├── __init__.py
│   ├── app.py                  # Flask application
│   ├── static/
│   │   ├── css/
│   │   │   └── style.css
│   │   └── js/
│   │       └── main.js
│   └── templates/
│       └── dashboard.html
│
├── tests/                      # Test suite
│   ├── test_crypto.py
│   ├── test_analysis.py
│   └── test_integration.py
│
├── sample_files/               # Sample files for demo
│   ├── sample.txt
│   └── sample2.txt
│
├── output/                     # Generated outputs (graphs, signatures)
│   └── .gitkeep
│
├── requirements.txt
├── run.py                      # Main entry point
└── README.md
```

---

## 🔧 Technical Stack

| Component | Technology |
|-----------|-----------|
| **Backend** | Python 3.8+ |
| **Cryptography** | `rsa`, `hashlib` (SHA-256) |
| **Performance** | `time`, `matplotlib` |
| **Frontend** | Flask + HTML/CSS/JS |
| **Visualization** | Matplotlib, Chart.js |

---

## 🚀 Quick Start

### 1. Clone the repository
```bash
git clone https://github.com/Atomiicradius/RSA-based-Document-Signature-Verification-System.git
cd RSA-based-Document-Signature-Verification-System
```

### 2. Create a virtual environment
```bash
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Run the application
```bash
python run.py
```

The dashboard will be available at `http://localhost:5000`

---

## 🎯 Core Features

### 1. Document Signing
- Upload files (.txt, .pdf)
- Generate SHA-256 hash
- Encrypt hash using RSA private key
- Export digital signature (.sig file)

### 2. Document Verification
- Upload original file + signature + public key
- Decrypt signature and compare hashes
- ✅ Valid / ❌ Invalid result display

### 3. Performance Analysis
- Time vs File Size graphs (hashing, signing, verification)
- Time vs Key Size comparison (512/1024/2048-bit RSA)
- Real-time benchmarking with matplotlib

### 4. Attack Simulation
- One-click file tampering
- Hash difference visualization
- Verification failure demonstration

### 5. Avalanche Effect
- Modify 1 character → see drastic hash change
- Bit-level difference percentage
- Side-by-side hash comparison

### 6. Secure Transfer Simulation
- Sender: upload + sign file
- Receiver: verify file + signature
- Visual step-by-step pipeline

---

## 👥 Team

| Role | Responsibility |
|------|---------------|
| **Person 1** | Cryptography Core (RSA, SHA-256, Sign/Verify) |
| **Person 2** | Analysis + Simulation (Performance, Attacks, Avalanche) |
| **Person 3** | UI + Integration (Flask Dashboard, UX) |

---

## 📄 License

This project is for educational purposes as part of the DAA EL project.
