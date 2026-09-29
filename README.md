🇷🇺 [Читать на русском](README_RU.md)

A full-stack web application featuring a deterministic probabilistic gaming simulation, cryptographic credential storage, and two-factor authentication (2FA) via a dedicated Telegram bot bridge.

### Key Architectural Highlights:
* **Telegram-Backed 2FA Verification:** Hybrid web-to-bot identity verification issuing one-time password (OTP) codes to the user's verified Telegram ID upon authentication.
* **Cryptographic Credential Hashing:** Secure salted password persistence backed by Werkzeug cryptographic primitives preventing rainbow table and plaintext exposures.
* **Probabilistic State Machine:** Dynamic roulette calculation engine tracking session balances, stake distributions, and historical transaction logs.
* **Cloud-Optimized Infrastructure:** Production-configured WSGI application designed for deployment across PythonAnywhere environments.

### Tech Stack:
* Python 3.12
* Flask (Microframework architecture)
* Werkzeug Security (Cryptographic hashing algorithms)
* SQLite (Relational user and betting ledger)
* Telegram Bot API (Out-of-band 2FA dispatch channel)

### Quick Start:
```bash
pip install -r requirements.txt
python flask_app(7).py
