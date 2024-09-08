# Deel Protocol
A decentralized Web3 freelance platform that connects KYC-verified users, enables cross-chain payments, and features secure messaging, attestation, and reputation systems.

## Overview

Deel Protocol is designed to bridge freelancers and clients within a secure, decentralized ecosystem. The platform ensures authenticity and trustworthiness through a KYC (Know Your Customer) process, creating a space where freelancers and clients can collaborate with confidence. 



## Repository Structure
We have two submodules :
- The `deel-sc` repository is the smart contract repository.
- The `deel-ui` repository is the frontend repository.

## Partners Intergated
- **Kinto**: We have used Kinto to have a KYC for both the job poster and the job applier. This is crucial for our application as both the job applier and the job poster must be KYCed to ensure compliance. Kinto is used at the very beginning of our product lifecycle when the user has to create his DEEL ID. Only after verifying through Kinto a user gets to complete his verification and gets onboarded into our application. 
- **Sign Protocol**: Sign Protocol is used to attest that work has been completed through the contractor and the job poster needs to attest that the work has been completed as well. For this matter two functions are used here: claimCompletedWork() and confirmCompletedWork, which are both used by different wallet addresses from either the job poster or the contractor.
- **XMTP**: We have used XMTP to create one-to-one conversations between the job poster and the job applicant. Transaction receipts can also be shared in the chat. This is a crucial feature for our platform because without conversation, improvements are not possible.
- **Chainlink**: CCIP is used for cross chain payments, messaging and attestations. We designed the protocol to be 1:N contracts where the 1 contract is considered the Main repository and Reciever of the protocol state. The N contracts are deployed across multiple chains that use their corresponding Routers to cross updates to the Main Reciever contract..All the contracts have the same source but act as a Sender or Reciever depending on the chain they are deployed.   Base sepolia being the main chain.
- **Morph**: We have used Morph to deploy our smart contracts. We have chosen Morph since our application is very consumer focused, which aligns perfectly with Morph's mission! We would be glad to build even more great consumer apps in the future during the ETHGlobal hackathons and hope Morph will be a sponsor yet again. 


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

## Morph
Contract: DeelProtocol
Address: 0xC924276a1D827b5E30655fBA6a66195644b070dE

## BaseSepolia 
Contract: DeelProtocol 
Address: 0xe43d0A3ebBbDb183A8eD9E2df91177F0B234d7AF

## Arbutrum Sepolia 
Contract: arbitrum Sepolia 
Address: 0x029d95963354be45230E9105597abE08e6cA6F7b




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
* Morph Holesky


#
