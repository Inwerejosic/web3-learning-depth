**Day 1** of your Solana Web3 engineering training 🚀.

**Blockchain basics** and comparing **Ethereum vs Solana**.

---

# 🔹 1. Blockchain Basics

At its core, a **blockchain** is:

* A **distributed ledger** (database shared across many computers).
* **Immutable** (you can only add data, not change past data).
* **Decentralized** (no single entity controls it fully).
* **Consensus-driven** (network participants agree on the "truth" of the ledger).

### Key concepts:

* **Block:** A batch of transactions bundled together.
* **Chain:** Blocks are linked together cryptographically (via hashes).
* **Node:** A computer running blockchain software to validate/relay transactions.
* **Consensus:** The protocol nodes use to agree on the state of the ledger (e.g., Proof of Work, Proof of Stake).

---

# 🔹 2. Ethereum Basics

Ethereum is a **general-purpose smart contract platform**.

### Key Features:

* **Smart Contracts:** Programs that run on-chain (written in Solidity/Vyper).
* **EVM (Ethereum Virtual Machine):** Executes smart contract bytecode.
* **Gas Fees:** Users pay fees (in ETH) to run transactions/smart contracts.
* **Consensus:**

  * Originally **Proof of Work (PoW)**,
  * Now **Proof of Stake (PoS)** (since "The Merge" in 2022).

👉 Ethereum prioritizes **decentralization & security** but often sacrifices **speed & scalability**.

---

# 🔹 3. Solana Basics

Solana is a **high-performance blockchain** designed for speed & scalability.

### Key Features:

* **Parallel Processing:** Unlike Ethereum, Solana can process multiple transactions at once.
* **Proof of History (PoH):** A cryptographic clock that orders transactions efficiently.
* **Low Fees:** Usually fractions of a cent per transaction.
* **High Throughput:** Capable of handling **65,000+ TPS (theoretical)**.
* **Programming Model:** Smart contracts are written in **Rust, C, or C++** (compiled to Berkeley Packet Filter bytecode, executed by Solana runtime).

👉 Solana prioritizes **scalability & speed**, sometimes trading off on **decentralization**.

---

# 🔹 4. Ethereum vs Solana – Key Differences

| Feature                    | **Ethereum**                                          | **Solana**                                            |
| -------------------------- | ----------------------------------------------------- | ----------------------------------------------------- |
| **Consensus**              | Proof of Stake (after Merge)                          | Proof of History + Proof of Stake                     |
| **TPS (Transactions/sec)** | \~30 TPS                                              | Up to 65,000+ TPS                                     |
| **Fees**                   | High (\$0.50–\$20+)                                   | Very low (< \$0.01)                                   |
| **Programming Language**   | Solidity, Vyper                                       | Rust, C, C++                                          |
| **Execution Model**        | Sequential (EVM processes transactions one at a time) | Parallel execution (via Sealevel runtime)             |
| **Decentralization**       | Highly decentralized                                  | Less decentralized (fewer validators compared to ETH) |
| **Ecosystem**              | Very mature (DeFi, NFTs, DAOs, L2s)                   | Growing fast (DeFi, NFTs, gaming)                     |

---

# 🔹 5. Code Examples

### Ethereum (Solidity)

```solidity
// Simple storage contract in Solidity
pragma solidity ^0.8.0;

contract Storage {
    uint256 number;

    function set(uint256 _number) public {
        number = _number;
    }

    function get() public view returns (uint256) {
        return number;
    }
}
```

### Solana (Rust)

```rust
// Example Solana program in Rust
use solana_program::{
    account_info::AccountInfo,
    entrypoint,
    entrypoint::ProgramResult,
    pubkey::Pubkey,
};

entrypoint!(process_instruction);

fn process_instruction(
    _program_id: &Pubkey,
    _accounts: &[AccountInfo],
    _instruction_data: &[u8],
) -> ProgramResult {
    msg!("Hello, Solana!");
    Ok(())
}
```

---

# 🔹 6. Further Reading

* **General Blockchain**

  * [Blockchain Basics (IBM)](https://www.ibm.com/topics/what-is-blockchain)
  * [Mastering Bitcoin (Free Book)](https://github.com/bitcoinbook/bitcoinbook)

* **Ethereum**

  * [Ethereum.org – Introduction](https://ethereum.org/en/developers/docs/intro-to-ethereum/)
  * [Solidity Docs](https://docs.soliditylang.org/)

* **Solana**

  * [Solana Docs](https://docs.solana.com/)
  * [Solana Cookbook (Developer Guide)](https://solanacookbook.com/)
  * [Solana Programming Model](https://docs.solana.com/developing/programming-model/overview)

---

