## What is Consensus in Bitcoin?

Consensus means **all participants (nodes/miners) in the Bitcoin network agree on a single, valid version of the blockchain**—without needing a central authority.  
It ensures:

- Everyone agrees on which transactions are valid.
- Double spending is prevented.
- The network remains secure and trust-less.

---
## Consensus Protocol of Bitcoin

### 1. **Proof of Work (PoW)**

- Core mechanism Bitcoin uses.
- Miners solve a **cryptographic puzzle** (find a hash below a target value).
- This requires **computational power and energy**.
- The first miner to solve it gets the right to add the next block and is rewarded with **block reward + transaction fees**.

#### Why PoW?
- Makes it **costly** to cheat.
- An attacker would need >50% of total network power (**51% attack**) to manipulate the chain, which is extremely expensive.
---
### 2. **Longest Chain Rule**

- Nodes always consider the **longest valid chain** (with most cumulative work) as the true blockchain.
- If two miners find a block at the same time → a fork happens.
- The fork is resolved when another block is added, making one chain longer. The shorter one is discarded.
---
### 3. **Block Validation**

**Before adding a block, nodes check:**
- Transactions are valid.
- No double spending.
- Block follows Bitcoin rules (correct size, correct nonce, correct difficulty, etc.).
---
### 4. **Difficulty Adjustment**

- Every **2016 blocks (~2 weeks)**, Bitcoin adjusts mining difficulty so blocks continue being produced every ~10 minutes, regardless of how many miners join/leave.
---
## Key Properties Achieved

1. **Security** – attackers need huge resources to alter blockchain.
2. **Decentralization** – no single authority, many miners compete.
3. **Finality** – after ~6 confirmations (~1 hour), transactions are practically irreversible.

---

## Summary

- **Bitcoin Consensus = Proof of Work + Longest Chain Rule + Difficulty Adjustment.**
- It ensures all nodes agree on a single blockchain, prevents fraud, and keeps the system decentralized and trust-less.

[[Proof of work]]