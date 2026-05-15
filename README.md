# 🏦 Bank Management system App

A simple banking application built with **Streamlit** and Python, allowing users to manage bank accounts through a clean web interface.

---

## Features

- **Create Account** — Register a new bank account with name, age, email, and a 4-digit PIN
- **Deposit** — Add funds to an existing account
- **Withdraw** — Withdraw funds from an existing account
- **Show Details** — View account information in JSON format
- **Update Info** — Update name, email, or PIN
- **Delete Account** — Permanently remove an account

---

## Project Structure

```
├── app.py        # Streamlit frontend
├── Bank.py       # Bank logic and data handling
├── data.json     # Local JSON file for persistent account storage
└── README.md
```

---

## Requirements

- Python 3.7+
- Streamlit

Install dependencies:

```bash
pip install streamlit
```

---

## Getting Started

1. Clone or download the repository.
2. Install the required packages (see above).
3. Run the app:

```bash
streamlit run app.py
```

4. Open your browser and go to `http://localhost:8501`.

---

## Usage

Use the **sidebar** to navigate between actions:

| Action | Description |
|---|---|
| Create Account | Fill in your details and a 4-digit PIN to open an account |
| Deposit | Enter your account number, PIN, and amount to deposit |
| Withdraw | Enter your account number, PIN, and amount to withdraw |
| Show Details | View your full account details using account number and PIN |
| Update Info | Optionally update your name, email, or PIN |
| Delete Account | Permanently close your account |

> **Note:** Your account number is displayed after successful account creation — keep it safe!

---

## Data Storage

Account data is stored locally in a **`data.json`** file. Each account entry is saved as a JSON object and persists between sessions.

Example structure:

```json
[
  {
    "accountNo.": "123456",
    "name": "John Doe",
    "age": 25,
    "email": "john@example.com",
    "pin": 1234,
    "balance": 500
  }
]
```

> **Note:** `data.json` is created automatically when the first account is registered. Do not manually edit this file while the app is running.

---
