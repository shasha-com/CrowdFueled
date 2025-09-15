# CrowdFueled

A decentralised crowdfunding application backed by blockchain and smart contracts built in Solidity.

---

## Table of Contents

- [Overview](#overview)  
- [Features](#features)  
- [Tech Stack](#tech-stack)  
- [Architecture](#architecture)  
- [Getting Started](#getting-started)  
  - [Prerequisites](#prerequisites)  
  - [Installation](#installation)  
  - [Running Locally](#running-locally)  
- [Smart Contract](#smart-contract)  
- [Project Structure](#project-structure)   

---

## Overview

CrowdFueled is a crowdfunding platform that leverages blockchain technology to provide transparency and immutability. Campaigns are managed via smart contracts, ensuring that funds are handled securely according to the rules codified on-chain. Users can create campaigns, contribute funds, and track progress using a front-end interface.

---

## Features

- Create new crowdfunding campaigns  
- Contribute / donate to campaigns  
- Track funding goals and progress  
- Smart contract enforces rules (e.g. what happens when goal met or missed)  
- Transparent, tamper-proof ledger of contributions  

---

## Tech Stack

- **Smart Contract** — Solidity  
- **Frontend / Client** — Ionic / Angular (TypeScript)
- **Backend** - Firebase 
- **Cross-platform support** — Capacitor   
- **Project tools** — Node.js, npm  

---

## Architecture

1. **Frontend**: Angular + Ionic app, uses Capacitor to deploy across native/web targets.  
2. **Smart Contract**: Solidity code that defines campaign logic. Deployed to a compatible Ethereum (or EVM) blockchain.  
3. **Integration**: Frontend interacts with blockchain via Web3 / ethers.js / similar provider (configure RPC endpoints).  

---

## Getting Started

### Prerequisites

- Node.js (v14+ recommended)  
- npm or yarn  
- An Ethereum-compatible environment (solidity)  
- Wallet (e.g. MetaMask) for interacting with contracts  

### Installation

```bash
# Clone the repo
git clone https://github.com/shasha-com/CrowdFueled.git
cd CrowdFueled

# Install frontend dependencies
npm install
```

### Running Locally

1. **Compile & Deploy Smart Contract**  
   - Open `SolidityCode.txt` (or solidity file) and adjust parameters.  
   - Use a framework like **Solidity** to compile and deploy:  

   ```bash
   # Example using Hardhat
   npx hardhat compile
   npx hardhat run scripts/deploy.js --network localhost
   
### Smart Contract
- 
