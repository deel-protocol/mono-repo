# Deel Protocol
A decentralized Web3 freelance platform that connects KYC-verified users, enables cross-chain payments, and features secure messaging, attestation, and reputation systems.

## Overview

Deel Protocol is designed to bridge freelancers and clients within a secure, decentralized ecosystem. The platform ensures authenticity and trustworthiness through a KYC (Know Your Customer) process, creating a space where freelancers and clients can collaborate with confidence. 



## Repository Structure
We have two submodules :
- The `deel-sc` repository is the smart contract repository.
- The `deel-ui` repository is the frontend repository.

### Partners Intergated
- **Kinto**: .
- **Sign Protocol**: 
- **XMTP**: 
- **Chainlink**: 
- **Morph**: 

### Key Features:
- **KYC Verification**: All users undergo KYC verification via **Kinto**, ensuring a secure and fraud-free environment.
- **Cross-Chain Payments**: Freelancers and clients can transact using multiple cryptocurrencies across different blockchain networks through **Chainlink CCIP**.
- **Attestation System**: **Sign Protocol** is used to verify completed tasks and provide an immutable, transparent history of freelancer performance.
- **Reputation System**: Freelancers and clients can earn ratings and feedback to build their reputation, which is visible on the platform for increased trust.
- **Secure Messaging**: Communication between users is encrypted using **XMTP** to protect privacy.


# `deel-ui` Repo

This is built using
- NextJS
- TypeScript
- Wagmi
- viem
- IDKit
- TailwindCSS
- ShadCn
- Aceternity UI
  
## Getting Started

First install the dependencies:

```bash
pnpm i
#or
yarn
#or
npm i
```

Paste the project ids in the `.env`

Then, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Then, open `localhost:3000`


# `deel-sc` Repo

## Usage

### Installation

```shell
cp .env.example .env
npm install
npx hardhat compile
npx hardhat test
```

# Deployed contracts


## BaseSepolia 
Contract: DeelProtocol 
Address: 0xe43d0A3ebBbDb183A8eD9E2df91177F0B234d7AF


## Arbutrum Sepolia 
Contract: arbitrum Sepolia 
Address: 0x029d95963354be45230E9105597abE08e6cA6F7b

## Mroph
Contract: DeelProtocol
Address: 0xC924276a1D827b5E30655fBA6a66195644b070dE


# Code Organization

## Kinto
`cp hardhat/.env.example hardhat/.env`
hardhat/README.md

## Chainlink CCIP
`cp hardhat/.env.example hardhat/.env`
hardhat/README.md

Networks
* Sepolia
* Arbitrum Sepoli
* Optimism Sepolia


#
