[![solidity - v0.8.17](https://img.shields.io/static/v1?label=solidity&message=v0.8.17&color=2ea44f&logo=solidity)](https://github.com/ethereum/solidity/releases/tag/v0.8.17)
[![ethers.js - v5.7.2](https://img.shields.io/static/v1?label=ethers.js&message=v5.7.2&color=2ea44f&logo=ethers.js)](https://github.com/ethers-io/ethers.js/releases/tag/v5.7.2)
[![hardhat - v2.12.6](https://img.shields.io/static/v1?label=hardhat&message=v2.12.6&color=2ea44f&logo=hardhat)](https://github.com/NomicFoundation/hardhat)

# ChainWave 

ChainWave is a Web3 dApp by **Omanshi Kaushal** that lets anyone send me a 👋 and a short message on the Ethereum blockchain, with a chance to win a small ETH reward on each wave. 

This project started from the classic WavePortal tutorial on buildspace and has been customized and extended to match my own style and ideas. 

<!-- Replace the line above with your live URL when deployed, for example:
https://chainwave.vercel.app  
-->   
 
## Tech Stack
 
- Solidity (smart contracts)
- Hardhat (development & testing) 
- Ethers.js (contract interaction)
- React.js (frontend)
- MetaMask (wallet)
- QuickNode / similar Ethereum node provider

## Getting Started

### 1. Clone the repository
git clone https://github.com/Omanshi19/ChainWave.git
cd ChainWave

### 2. Install dependencies
npm install 

### 3. Environment variables
Create a `.env` file in the project root:
STAGING_QUICKNODE_KEY=https://your-quicknode-or-rpc-url
PROD_QUICKNODE_KEY=
PRIVATE_KEY=your_metamask_private_key

> Do **not** commit this file. It is already ignored by `.gitignore`. 

### 4. Run tests
npx hardhat test

### 5. Start a local Hardhat node
npx hardhat node

### 6. Deploy the contract locally
In a separate terminal:
npx hardhat run ./scripts/deploy.js --network localhost

### 7. Start the frontend
npm run start 

The app should now be available at `http://localhost:3000`.

## Project Notes

- Waves (messages) are stored on-chain via the `WavePortal` contract.
- There is a simple cooldown to prevent spamming and a pseudo-random reward mechanism for waves.
- This is a learning and experimentation project around Ethereum, not production financial software. 


