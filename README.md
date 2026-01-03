# Decentralized Exchange (DEX) with Automated Market Maker (AMM)

A production-ready implementation of a **Decentralized Exchange (DEX)** based on the **Constant Product Automated Market Maker (AMM)** model (Uniswap V2 style). This protocol enables trustless token swaps, decentralized liquidity provision, and transparent fee distribution.

## Overview

This project demonstrates the core mechanics of decentralized finance (DeFi). By utilizing the constant product formula (), the exchange ensures that liquidity is always available for traders without the need for a centralized order book.

### Key Features

* **Trustless Swaps:** Algorithmic token exchange using the Constant Product Formula.
* **Liquidity Management:** Minting and burning of LP tokens to track pool ownership.
* **0.3% Fee Protocol:** Built-in incentive mechanism that rewards liquidity providers.
* **Robust Testing:** 25+ test cases covering edge cases, math validation, and security.
* **Deterministic Environment:** Fully Dockerized setup for consistent development and deployment.

---

## Architecture

### Core Components

* `DEX.sol`: The engine of the protocol. Handles reserves, swaps, and LP accounting.
* `MockERC20.sol`: Standardized tokens used for testing and simulation.
* `Hardhat`: Used for compilation, local node simulation, and debugging.
* `Docker`: Ensures the environment is identical across all machines.

### Repository Structure

```text
dex-amm/
├── contracts/          # Smart Contracts (Solidity)
├── test/               # Hardhat Test Suite (JavaScript)
├── scripts/            # Deployment Scripts
├── Dockerfile          # Container Configuration
└── hardhat.config.js   # Hardhat Settings

```

---

##  Mathematical Foundation

The DEX relies on precise mathematical formulas to ensure economic stability:

| Action | Formula |
| --- | --- |
| **Price Discovery** |  |
| **Invariant** |  |
| **Swap Output** |  |
| **LP Minting** |  |

---

## Setup & Installation

### Prerequisites

* [Docker](https://www.docker.com/) & Docker Compose
* [Node.js](https://nodejs.org/) (Optional, for local-only dev)

### Quick Start with Docker

```bash
# Clone the repository
git clone https://github.com/sudheerimmidisetti/Build-Decentralized-Exchange-with-Automated-Market-Maker-Protocol.git
cd Build-Decentralized-Exchange-with-Automated-Market-Maker-Protocol

# Start the environment
docker-compose up -d

# Compile and Run Tests
docker-compose exec app npm run compile
docker-compose exec app npm test

```

### Local Development

```bash
npm install
npm run compile
npm test

```

---

## Security & Coverage

This project prioritizes smart contract security through:

* **Overflow Protection:** Native Solidity 0.8+ checked math.
* **Safe Transfers:** Implementation of OpenZeppelin’s `SafeERC20`.
* **Validation:** Strict checks on reserve ratios and slippage edge cases.
* **Test Coverage:** Targeted  code coverage for all core functions.

---

## Learning Outcomes

* Deep understanding of **AMM mechanics** and liquidity incentives.
* Mastery of **Hardhat** for Ethereum development workflows.
* Implementation of **ERC-20** standards and LP token logic.
* Proficiency in **Dockerizing** blockchain environments for CI/CD.

---
