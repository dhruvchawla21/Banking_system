# 🏦 SBI Banking System — Python OOP Project

A beginner-to-intermediate level **command-line banking system** built with Python, demonstrating core Object-Oriented Programming concepts like classes, objects, encapsulation, and instance methods — with realistic banking rules and edge cases.

---

## 📌 About the Project

This project simulates a simple bank account management system. It was built to practise OOP in Python by modelling real-world banking behaviour — not just basic get/set methods, but actual rules like minimum balance enforcement, PIN protection, transfer validation, and account lifecycle management.

---

## ✨ Features

| Feature | Description |
|---|---|
| 💳 Deposit | Add funds with an upper limit for large cash deposits |
| 🏧 Withdraw | Debit funds with PIN verification and minimum balance check |
| 🔁 Transfer | Move money between two accounts with full validation |
| 📋 Balance Enquiry | PIN-protected balance check with account details |
| 📜 Transaction History | View a log of all past transactions |
| 🔒 Close Account | Deactivate an account and pay out remaining balance |

---

## 🛡️ Validations & Edge Cases

The system enforces the following rules on every transaction:

- ❌ Wrong PIN blocks the operation entirely
- ❌ Amount must be greater than `0`
- ❌ Cannot withdraw more than the available balance
- ❌ A minimum balance of **Rs 1,000** must always be maintained
- ❌ Withdrawals must be in **multiples of Rs 100**
- ❌ Cash deposits above **Rs 1,00,000** require manager approval
- ❌ Transfers to a **closed account** are rejected
- ❌ No transactions are allowed on a **closed account**

---

## 🧠 OOP Concepts Used

```
Class & Object          →  Account class with multiple instances
Instance Attributes     →  balance, account_no, name, is_active
Class Attribute         →  bank_name, minimum_balance (shared across all accounts)
Encapsulation           →  __pin is a private attribute (name mangling)
Instance Methods        →  debit(), credit(), transfer(), etc.
Helper / Guard Methods  →  __verify_pin(), __check_active(), __log_transaction()
```

---

## 🗂️ Project Structure

```
banking-system/
│
├── banking_system.py   # Main source file with Account class and demo
└── README.md           # Project documentation
```

---

## 🚀 Getting Started

### Prerequisites
- Python 3.x (no external libraries needed)

### Run the project

```bash
# Clone the repository
git clone https://github.com/your-username/banking-system.git

# Navigate into the folder
cd banking-system

# Run the script
python banking_system.py
```

---

## 🖥️ Sample Output

```
═══════════════════════════════════════════════
   Welcome to State Bank of India (SBI)
═══════════════════════════════════════════════

─────────────────────────────────────────────
  📋  BALANCE ENQUIRY  |  A/C: 112233
─────────────────────────────────────────────
  Account Holder : Ravi Kumar
  Account No.    : 112233
  Bank           : State Bank of India (SBI)
  Balance        : Rs 10000
─────────────────────────────────────────────

─────────────────────────────────────────────
  🏧  WITHDRAWAL REQUEST  |  A/C: 112233
─────────────────────────────────────────────
  ✅  Rs 2000 debited successfully.
  💰  Remaining Balance : Rs 8000
─────────────────────────────────────────────
```

---

## 🔮 Possible Extensions

Want to take this further? Here are some ideas:

- [ ] Add multiple account types (Savings, Current, Fixed Deposit)
- [ ] Implement daily transaction limits
- [ ] Add interest calculation for savings accounts
- [ ] Store account data in a file (JSON / CSV) for persistence
- [ ] Build a simple CLI menu for interactive use
- [ ] Add timestamps to transaction history

---

## 👤 Author

**Your Name**  
[GitHub](https://github.com/your-username) · [LinkedIn](https://linkedin.com/in/your-username)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
