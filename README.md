# Omni-Hunt v1.0
## Advanced OSINT & Credential Awareness Testing Framework

<div align="center">

![Python](https://img.shields.io/badge/Python-3.8%2B-3776AB?style=for-the-badge&logo=python)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Research%20%2F%20PoC-orange?style=for-the-badge)
![Auth](https://img.shields.io/badge/Use-Authorized%20Security%20Research-blue?style=for-the-badge)

</div>

Omni-Hunt is a research-oriented OSINT and credential-awareness framework developed for authorized cybersecurity testing, controlled demonstrations, and ethical security awareness training.

The project is built around a modern authentication simulation workflow and includes:
- SMTP-based email verification
- DNS and MX resolution checks
- Gravatar profile enumeration techniques
- Real-time WebSocket communication
- Simulated Google-style login experience
- Structured telemetry and artifact logging for research review

---

## ⚠️ Ethical Use Notice

This project is intended only for:
- Authorized security assessments with explicit permission
- Ethical red-team testing in controlled environments
- Security awareness and training exercises
- Research-focused demonstrations in legally compliant scenarios

This project must not be used for:
- Unauthorized access
- Malicious phishing campaigns
- Credential theft or privacy violations
- Any illegal or unethical activity

The author does not endorse misuse of this project. Use responsibly and in full compliance with applicable laws and organizational policies.

---

## 🔍 Project Overview

Omni-Hunt was designed to demonstrate how identity validation and credential awareness workflows can be analyzed in a lab-style environment. It is structured as a practical research utility focused on ethical experimentation and awareness.

The framework combines multiple capabilities into a single demonstration platform:
- email existence validation
- profile enumeration via publicly accessible digital identity services
- dynamic front-end simulation of a real-world authentication flow
- telemetry and logging for post-engagement documentation

---

## 🚀 Key Features

- SMTP email verification using DNS and mail-server interaction
- MX record resolution for identity validation checks
- Gravatar-based profile image discovery
- Real-time WebSocket-based communication for telemetry events
- High-fidelity login UI simulation inspired by modern authentication providers
- Controlled logging of captured test data in a research environment
- Modular architecture for future expansion and experimentation

---

## 🧩 Architecture

```text
[Frontend Layer]
  └── Google-style UI simulation

[Application Layer]
  └── Python-based validation engine and WebSocket handler

[Data Layer]
  └── Generated artifacts, logs, and profile metadata
```

---

## 📦 Repository Structure

```text
omni-hunt/
├── README.md
├── LICENSE
├── .gitignore
├── requirements.txt
├── SETUP.md
├── CONTRIBUTING.md
├── intigrate.py
├── google1.html
├── static/
│   ├── default.jpg
│   ├── captured_credentials.txt
│   └── generated_profile_images/
└── docs/
    └── screenshots/
```

---

## 🛠️ Installation

### Prerequisites
- Python 3.8+
- pip
- Git
- Modern web browser

### Clone the repository

```bash
git clone https://github.com/hacksben/omni-hunt.git
cd omni-hunt
pip install -r requirements.txt
```

### Run the application

```bash
python intigrate.py
```

### Access the UI

Open the following URL in a browser:

```text
http://localhost:8000
```

---

## 📸 Proof of Concept (PoC)

This project includes a proof-of-concept demonstration showing:
1. application startup and telemetry initialization
2. email validation steps
3. simulated authentication flow
4. password capture demonstration in a controlled environment
5. generated artifacts and logs

The PoC is presented for educational, research, and authorized security testing purposes only.

> This repository focuses on the project structure, documentation, and professional presentation of the PoC workflow. The actual demonstration assets can be added separately by the project owner.

---

## 📜 License

This project is licensed under the MIT License.

See the `LICENSE` file for full details.

---

## 👨‍💻 Author

**MANDEEP PARMAR**

Cybersecurity Researcher | OSINT Enthusiast | Security Awareness Advocate

- Email: sparmar28332@gmail.com
- GitHub: https://github.com/hacksben
- LinkedIn: https://www.linkedin.com/in/mandeep-parmar-b73a54381
- Location: Sonipat, Haryana, India

---

## 🤝 Contribution Guidelines

Contributions, suggestions, and documentation improvements are welcome. Please review `CONTRIBUTING.md` before submitting changes.

---

## 🔐 Security Notice

Omni-Hunt is for authorized research and awareness activities only. All use must respect legal requirements, organizational policies, and privacy standards.

---

<div align="center">
  <strong>Made for ethical cybersecurity research and awareness.</strong>
</div>
