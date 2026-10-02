# Omni-Hunt PoC and MITRE ATT&CK Mapping

## Overview

This document maps the Omni-Hunt Proof of Concept flow to relevant MITRE ATT&CK techniques to provide a structured security research perspective.

---

## Mapping Summary

| Technique ID | Tactic | Technique Name | Relevance to Omni-Hunt |
|---|---|---|---|
| T1566.002 | Initial Access | Phishing: Spearphishing Link | Demonstrates how a credential submission interface can appear authentic |
| T1589.002 | Reconnaissance | Gather Victim Identity: Email Addresses | Email validation and identity checking are central to the project workflow |
| T1071.001 | Command and Control | Application Layer Protocol: Web Protocols | WebSocket communication supports telemetry and event streaming |
| T1555.005 | Credential Access | Credentials from Password Stores | Demonstrates credential capture in a controlled research environment |

---

## Research Interpretation

The project demonstrates a structured simulation of security research, awareness validation, and controlled authentication testing. It is important to frame the workflow as a legitimate educational and authorized security exercise rather than a toolkit for unauthorized malicious activity.

---

## Ethical Use Statement

The MITRE mapping is included to provide context and demonstrate the operational logic behind the PoC, not to encourage misuse or malicious exploitation.

---

## Author

- MANDEEP PARMAR
- Email: sparmar28332@gmail.com
- LinkedIn: https://www.linkedin.com/in/mandeep-parmar-b73a54381
- GitHub: https://github.com/hacksben
