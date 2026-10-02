# Omni-Hunt Setup Guide

This document provides setup instructions for the Omni-Hunt project and its research-focused environment.

---

## Prerequisites

Before running the project, make sure the following are available:

- Python 3.8 or higher
- pip package manager
- Git
- Modern browser

---

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/hacksben/omni-hunt.git
cd omni-hunt
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Run the application

```bash
python intigrate.py
```

### 4. Open the interface

Visit:

```text
http://localhost:8000
```

---

## Troubleshooting

### Module not found

If Python modules are missing, install them manually:

```bash
pip install websockets dnspython
```

### Port already in use

If localhost ports 8000 or 8080 are already active, stop the existing service or adjust the port configuration in the project files.

---

## Security Reminder

Run the project only in a controlled, authorized environment. Always ensure the testing environment has valid consent and legal approval before use.
