# 📝 Stellar Ledger

The Stellar Ledger is the immutable, distributed record of all account balances, transactions and state on the Stellar network[43dcd9a7-70db-4a1f-b0ae-981daa162054](https://digidollar.org/article/detail/what-is-stellar/?citationMarker=43dcd9a7-70db-4a1f-b0ae-981daa162054 "1"). It underpins Stellar’s mission to enable fast, low-cost cross-border payments by maintaining:

- A sequential series of **ledger headers** (sequence number, close time, transaction set hash)  
- A set of **state entries** (accounts, offers, trustlines)  
- A list of **transactions** applied in each ledger close  
- Cryptographic proofs and signatures produced by the Stellar Consensus Protocol (SCP) to guarantee finality[43dcd9a7-70db-4a1f-b0ae-981daa162054](https://digidollar.org/article/detail/what-is-stellar/?citationMarker=43dcd9a7-70db-4a1f-b0ae-981daa162054 "1")

---

## 🚀 Key Concepts

- Ledger Sequence  
  Each closed ledger increments a global sequence number and ties together its header, the prior ledger’s hash, and the root of its state Merkle tree.

- Ledger Header  
  Contains metadata for consensus: sequence, time bounds, previous ledger hash, transaction-set hash, and SCP‐generated signatures.

- State Entries  
  Persist account data (balances, signers, thresholds), trustlines, offers, data entries, and more—indexed by a 256-bit key.

- Transactions & Operations  
  Each transaction bundles one or more operations (payments, path payments, trustline changes) and is applied atomically at close time.

- Stellar Consensus Protocol (SCP)  
  Nodes federate consensus via Quorum Slices and Federated Byzantine Agreement (FBA), securing each ledger close without proof-of-work[43dcd9a7-70db-4a1f-b0ae-981daa162054](https://digidollar.org/article/detail/what-is-stellar/?citationMarker=43dcd9a7-70db-4a1f-b0ae-981daa162054 "1").

---

## 📂 Repository Structure# Stellar-ledger
