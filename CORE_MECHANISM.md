# CORE_MECHANISM.md

## 🌐 StarPay – Core Operational Mechanism (XCB-Powered Cross-Border Payment)

This document outlines the internal operation logic and core mechanism of the StarPay system. It complements the whitepaper and funding plan.

---

## 🔁 1. Non-Cross-Border Settlement Model

Traditional cross-border payments involve transferring funds internationally, leading to legal complexity, delay, and high costs. StarPay replaces this with a **"user data + liquidity sync"** mechanism.

- Funds do not leave the source country.
- User balance data is migrated across **national nodes**.
- Local fund movement is executed via **local smart contracts**.

---

## 🏛 2. Node Architecture

StarPay deploys three types of nodes:

1. **User Nodes**
   - Wallets and StarPay Apps
   - Store balance data, trigger transactions

2. **National Nodes**
   - Local XCB reserve management
   - Execute liquidity routing & KYC

3. **Main DAO Node**
   - Smart contract governance
   - Regulatory interface & oversight

---

## 🔐 3. Smart Contract Governance

- All fund logic is enforced by contracts:
  - Transfer permissions
  - Tax or fee deduction
  - Emergency freeze mechanism

- DAO sets logic, government can view results but cannot intervene

---

## 💱 4. Liquidity & Exchange Model

- 1 XCB = 1.05 USDT (user buy)
- 1 XCB = 0.95 USDT (user sell)
- Spread supports platform sustainability

Local banks or partner exchanges integrate XCB on/off ramp with real-world currencies.

---

## 💰 5. Revenue Flow

| Source | Fee | Recipient |
|--------|-----|-----------|
| User-to-User Payment | 0.5% | Platform DAO |
| XCB Conversion | Spread (5–10%) | Platform Reserve |
| Government Option | 10–20% | Local governments (if accepted) |

---

## 📊 6. Transparency & Query

- All data is recorded on-chain
- Users and regulators can query via gas-efficient contracts
- Batch queries supported

---

## ⚙️ 7. MVP & Simulation Logic

- Simulation module allows API testing
- Developers can submit scenarios
- Feedback delivered within 30s

---

## 🧠 8. Sub-Island Modularity

- All functions are modular:
  - KYC plugin
  - Tax logic
  - AML scan
  - User interface pack

Future developers can create plugins under Star DAO rules.

---

## 📁 Files Reference

- `README.md: Project overview
- `XCB_Funding_Proposal.md: Investment and budget
- `project_diagram.png: Visual architecture

---

**Version:** Draft v0.1 – for community review  
**Maintainer:** STARPAY Team / hakbong.oh  
