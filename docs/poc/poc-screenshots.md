# Omni-Hunt PoC - Visual Screenshots

## Overview

This document contains professional visual representations of the Omni-Hunt Proof of Concept workflow, demonstrating each stage of the system in a controlled security research environment.

---

## Screenshot 1: Terminal Initialization and Backend Startup

### Stage Description
The initial phase shows the Omni-Hunt backend engine starting up, initializing services, and preparing the environment for the demonstration.

### Visual Representation

```
┌─────────────────────────────────────────────────────────────────────┐
│ $ python3 intigrate.py                                              │
│                                                                     │
│ [*] Default avatar downloaded                                       │
│ [*] Target WebSocket engine spinning up on ws://localhost:8080     │
│ [*] UI Frontend Server started on http://localhost:8000            │
│ [*] Profile pictures saved to: /home/mandeep/omni-hunt/static      │
│ [*] Credentials will be saved to:                                  │
│     /home/mandeep/omni-hunt/static/captured_credentials.txt        │
│                                                                     │
│ ✓ Services initialized successfully                                 │
│ ✓ Awaiting browser connection...                                    │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

### Technical Notes
- Backend initialization completes successfully
- WebSocket server ready on port 8080
- HTTP interface available on port 8000
- Static directory prepared for artifacts
- System ready for demonstration

### Professional Interpretation
This screenshot demonstrates the proper startup sequence and confirms that all services are operational and ready to begin the credential-awareness demonstration in a controlled environment.

---

## Screenshot 2: Google-Style Sign-In Interface - Email Entry Stage

### Stage Description
The user is presented with a professional, Google-inspired login interface designed to simulate a familiar modern authentication flow.

### Visual Representation

```
┌─────────────────────────────────────────────────────────────────────┐
│                                                                     │
│                          [Google Logo]                              │
│                                                                     │
│                           Sign in                                   │
│                      Use your Google Account                        │
│                                                                     │
│  ┌──────────────────────────────────────────────────────────────┐  │
│  │                                                              │  │
│  │  Email or phone                                             │  │
│  │  ___________________________________                         │  │
│  │                                                              │  │
│  └──────────────────────────────────────────────────────────────┘  │
│                                                                     │
│                     [Forgot email?]                                 │
│                                                                     │
│  Not your computer? Use Guest mode to sign in privately.            │
│  Learn more about using Guest mode                                  │
│                                                                     │
│              [Create account]          [Next →]                     │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

### User Experience Flow
1. User lands on sign-in page
2. Professional branding and layout
3. Email input field ready for entry
4. Clear next-step action button
5. Realistic UI patterns

### Professional Interpretation
This screenshot represents the first interactive stage where the target email is entered. The interface mimics modern authentication providers, creating a familiar environment for the demonstration.

---

## Screenshot 3: Authentication Flow - Password Entry Stage

### Stage Description
After email validation, the system transitions to the password collection stage, displaying enumerated profile information to increase realism.

### Visual Representation

```
┌─────────────────────────────────────────────────────────────────────┐
│                                                                     │
│                          [Google Logo]                              │
│                                                                     │
│                           Welcome                                   │
│                                                                     │
│  ┌──────────────────────────────────────────────────────────────┐  │
│  │  ┌──────┐                                                    │  │
│  │  │[Pic] │  test.user@gmail.com                        ▼      │  │
│  │  └──────┘                                                    │  │
│  └──────────────────────────────────────────────────────────────┘  │
│                                                                     │
│  ┌──────────────────────────────────────────────────────────────┐  │
│  │                                                              │  │
│  │  Enter your password                                        │  │
│  │  •••••••••••••••••••••••                                    │  │
│  │                                                              │  │
│  └──────────────────────────────────────────────────────────────┘  │
│                                                                     │
│  ☐ Show password                                                   │
│                                                                     │
│           [Try another way]          [Next →]                      │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

### Technical Implementation
- Profile picture displayed (enumerated via Gravatar)
- Email confirmed from previous stage
- Password field with standard masking
- Show/hide password toggle available
- Secondary authentication options presented

### Professional Interpretation
This stage demonstrates the seamless transition in a credential-awareness simulation, showing how familiar UI patterns and profile pictures increase user trust in a controlled research environment.

---

## Screenshot 4: Real-Time Telemetry and Backend Activity Logging

### Stage Description
While the user interaction is occurring, the backend system logs all validation activities and events to the terminal in real-time.

### Visual Representation

```
┌─────────────────────────────────────────────────────────────────────┐
│ $ python3 intigrate.py                                              │
│ [...initialization logs...]                                         │
│                                                                     │
│ [*] Browser connected successfully via WebSocket protocol           │
│ [*] Verifying target: test.user@gmail.com                          │
│ [+] Profile picture saved for test.user                             │
│ [+] Result sent back to UI for test.user@gmail.com: found          │
│ [*] Waiting for password input...                                   │
│                                                                     │
│ [*] Password received for: test.user@gmail.com                     │
│ [+] Credentials saved for test.user@gmail.com                       │
│                                                                     │
│ [*] Writing to artifact file...                                    │
│ [+] File write complete: captured_credentials.txt                   │
│                                                                     │
│ [*] Session logging complete                                        │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

### Event Flow
- Real-time telemetry streaming
- Email validation confirmation
- Profile enumeration status
- Credential capture logged
- Artifact file generation
- Session completion

### Professional Interpretation
This screenshot shows the backend operational transparency, demonstrating how all system activities are logged, monitored, and documented for post-engagement analysis.

---

## Screenshot 5: Generated Artifacts and Credential Log File

### Stage Description
The system generates a structured artifact file containing captured credentials with timestamps, suitable for post-engagement review and documentation.

### Visual Representation

```
File: static/captured_credentials.txt

┌─────────────────────────────────────────────────────────────────────┐
│ ========== OMNI-HUNT CREDENTIAL CAPTURE LOG ==========               │
│                                                                     │
│ [2026-10-02 14:32:18] Email: test.user@gmail.com                   │
│                       Password: P@ssw0rd!                            │
│                       Status: Captured                               │
│                       Profile: Found (Gravatar Enumerated)           │
│                                                                     │
│ [2026-10-02 14:35:42] Email: mandeep@example.com                   │
│                       Password: Secure123                            │
│                       Status: Captured                               │
│                       Profile: Not Found                             │
│                                                                     │
│ ========== END OF LOG ==========                                     │
│                                                                     │
│ Total Entries: 2                                                    │
│ Session Duration: 3m 24s                                            │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

### Artifact Details
- Timestamp-based entries
- Email and credential records
- Profile enumeration status
- Session metadata
- Structured logging format

### Professional Interpretation
This artifact demonstrates the structured output and documentation capability of the system, showcasing how captured data is organized and stored for later review in a research context.

---

## Screenshot 6: Project Directory Structure with Generated Files

### Stage Description
After the demonstration completes, the project directory contains organized artifacts ready for analysis.

### Visual Representation

```
omni-hunt/
├── README.md
├── LICENSE
├── requirements.txt
├── SETUP.md
├── CONTRIBUTING.md
├── intigrate.py
├── google1.html
├── static/
│   ├── default.jpg                    # Default profile avatar
│   ├── test.user.jpg                  # Enumerated Gravatar image
│   ├── mandeep.jpg                    # Enumerated Gravatar image
│   └── captured_credentials.txt       # Main artifact log
├── docs/
│   ├── screenshots/                   # This documentation
│   └── poc/
│       ├── poc-overview.md
│       ├── poc-stages.md
│       ├── poc-screenshots.md
│       ├── poc-results.md
│       └── poc-mitre-mapping.md
└── .gitignore
```

### Professional Interpretation
The organized directory structure demonstrates professional project management and artifact organization, making it easy for security teams to review and document findings post-engagement.

---

## Summary of PoC Workflow

The screenshot sequence documents a complete Omni-Hunt demonstration:

1. **Initialization** - Backend services start successfully
2. **User Interface** - Professional sign-in page presents
3. **Email Validation** - Target identity is processed
4. **Password Entry** - Credential submission stage begins
5. **Real-Time Logging** - Backend tracks all activities
6. **Artifact Generation** - Results are stored and organized
7. **Documentation** - Professional output ready for review

---

## Security and Ethical Context

All screenshots and demonstrations are presented in the context of:
- Authorized security research
- Controlled lab environments
- Explicit user consent scenarios
- Educational and awareness purposes
- Legal compliance frameworks

---

## Author

**MANDEEP PARMAR**

- Email: sparmar28332@gmail.com
- GitHub: https://github.com/hacksben
- LinkedIn: https://www.linkedin.com/in/mandeep-parmar-b73a54381
- Location: Sonipat, Haryana, India

---

## Project Links

- Repository: https://github.com/hacksben/omni-hunt
- Main Documentation: See `README.md`
- Setup Guide: See `SETUP.md`
- Contributing: See `CONTRIBUTING.md`

---

<div align="center">
  <strong>Made for ethical cybersecurity research and awareness.</strong>
</div>
