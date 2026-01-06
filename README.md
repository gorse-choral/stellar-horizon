# Stellar Horizon (For Base)

Stellar Horizon is a simple, read-only tool designed for inspecting and validating the Base Sepolia network. It helps developers verify network status, inspect wallet balances, and validate contract deployments without making any state-changing operations.

---

## Key Features

Stellar Horizon provides the following functionality:
- Verify the connection to Base Sepolia (chainId: 84532)  
- Inspect wallet balances and transaction details  
- Validate contract deployments with direct Basescan links  
- Review block and gas usage data  

This tool only performs read-only actions, ensuring no impact on the blockchain.

---

## How It Works

Stellar Horizon connects to Coinbase Wallet using the Coinbase Wallet SDK and communicates with the Base Sepolia network via the viem library. It retrieves onchain data such as wallet balances, transaction counts, block information, and gas prices, and offers verified explorer links for confirmation.

No transactions are signed or broadcasted.

---

## Repository Structure

- **app/stellar-horizon.ts**  
  The primary script that connects to Coinbase Wallet and queries Base Sepolia for blockchain data.

- **contracts/**  
  Solidity contracts deployed on Base Sepolia for testnet validation:
  - `ERC721.sol`  
  - `control.sol`  
  - `storage.sol`  

- **logs/**  
  Contains logs of network checks and testnet validations:
  - `execution.log`  

- **package.json**  
  Contains dependencies for the project.

- **README.md**  
  The main documentation file.

---

## Supported Networks

Base Sepolia  
chainId (decimal): 84532  
Explorer: [sepolia.basescan.org](https://sepolia.basescan.org)

---

## Network Information

The tool allows you to verify the connection to the Base Sepolia network. It retrieves information like:
- Wallet balance
- Transaction counts
- Contract details
- Block number and gas usage

This information helps ensure that everything is working correctly on the Base Sepolia network.

---

## Dependencies

Stellar Horizon uses the following dependencies:
- **Coinbase Wallet SDK** for wallet integration  
- **Viem** for interacting with the Base network  
- **Axios** for making HTTP requests  
- **Web3** for extended wallet functionality  
- **Ethers.js** for Ethereum protocol interaction  

---

## Testnet Deployments (Base Sepolia)

These contracts have been deployed on Base Sepolia for validation and testing:

Network: Base Sepolia  
chainId (decimal): 84532  
Explorer: [sepolia.basescan.org](https://sepolia.basescan.org)

Contract ERC721.sol address:  
0x9855a2e65C1B17B8F9B5E9DD64F6b1d44D668dE2

Deployment and verification:
- [Deployment Link](https://sepolia.basescan.org/address/0x9855a2e65C1B17B8F9B5E9DD64F6b1d44D668dE2)
- [Code Verification](https://sepolia.basescan.org/0x9855a2e65C1B17B8F9B5E9DD64F6b1d44D668dE2/0#code)

Contract control.sol address:  
0x140528b5565815c23f8c5dC55fC18840c45f328f

Deployment and verification:
- [Deployment Link](https://sepolia.basescan.org/address/0x140528b5565815c23f8c5dC55fC18840c45f328f)
- [Code Verification](https://sepolia.basescan.org/0x140528b5565815c23f8c5dC55fC18840c45f328f/0#code)

Contract storage.sol address:  
0xa826F197A0f25b84d615275D50a85146d3c5e7Fd

Deployment and verification:
- [Deployment Link](https://sepolia.basescan.org/address/0xa826F197A0f25b84d615275D50a85146d3c5e7Fd)
- [Code Verification](https://sepolia.basescan.org/0xa826F197A0f25b84d615275D50a85146d3c5e7Fd/0#code)


These deployments help validate the Base Sepolia network, ensuring compatibility with the tooling before mainnet usage.

## License

MIT License  
Copyright (c) 2025 YOUR_NAME

---

## Author

GitHub: [gorse-choral](https://github.com/gorse-choral)  

Email: 03-gorse-choral@icloud.com

Twitter: https://x.com/vilmerbeast676
