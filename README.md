# Decentralized Task Manager

A **Decentralized Task Manager** is a blockchain-powered task management system that enables users to create, assign, and track tasks transparently and securely without relying on a central authority. Built on Ethereum, this platform ensures immutability, transparency, and fair collaboration among users.

## Features

- ✅ **Decentralized & Trustless** – No central authority; all task data is stored on the blockchain.
- 🔗 **Smart Contracts** – Ethereum-based smart contracts handle task creation, assignment, and completion.
- 🔐 **Secure & Transparent** – Every action is recorded immutably on the blockchain.
- 👥 **Role-Based Access** – Users can create, assign, and manage tasks based on predefined roles.
- 💰 **Crypto Payments** – Reward system using cryptocurrency for task completion.
- 🛠️ **Interoperability** – Compatible with Web3 wallets like MetaMask.

## Tech Stack

- **Smart Contracts**: Solidity, Hardhat
- **Blockchain**: Ethereum / Polygon (for lower gas fees)
- **Frontend**: React.js, Next.js
- **Backend**: Node.js, Express
- **Database**: IPFS (for decentralized storage)
- **Authentication**: Web3.js / Ethers.js (MetaMask integration)

## Getting Started

### Prerequisites

- Node.js (>= 16)
- npm or yarn
- MetaMask Wallet
- Ethereum Testnet (Goerli / Sepolia) for testing

### Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/decentralized-task-manager.git
   cd decentralized-task-manager
   ```

2. Install dependencies:
   ```sh
   npm install  
   # or
   yarn install
   ```

3. Set up environment variables in `.env.local`:
   ```env
   NEXT_PUBLIC_INFURA_API_KEY=your_infura_project_id
   NEXT_PUBLIC_CONTRACT_ADDRESS=your_deployed_contract_address
   ```

4. Compile and deploy smart contracts to a testnet:
   ```sh
   npx hardhat compile
   npx hardhat run scripts/deploy.js --network goerli
   ```

5. Start the frontend:
   ```sh
   npm run dev  
   # or
   yarn dev
   ```

6. Open `http://localhost:3000` in your browser.

## Smart Contract Overview

The smart contract includes the following functions:
- `createTask(string memory _title, string memory _description, uint256 _reward)`
- `assignTask(address _assignee, uint256 _taskId)`
- `completeTask(uint256 _taskId)`
- `withdrawRewards()`

## Deployment

To deploy on **Ethereum Mainnet or Polygon**:
1. Update `.env.local` with the mainnet RPC URL.
2. Deploy contracts using:
   ```sh
   npx hardhat run scripts/deploy.js --network mainnet
   ```
3. Deploy the frontend on Vercel or Netlify.

## Contributing

1. Fork the repository.
2. Create a feature branch: `git checkout -b feature-branch`.
3. Make your changes and commit.
4. Push to your branch and create a PR.

## License

This project is licensed under the MIT License.

## Contact

For queries or collaborations, reach out:
- **Twitter**: [@whatever_ankit](https://x.com/whatever_ankit)
- **LinkedIn**: [Ankit Dhadiwal](https://www.linkedin.com/in/ankit-dhadiwal-8352a1229/)
- **GitHub**: [ankitdhadiwal](https://github.com/ankitdhadiwal)

🚀 Build decentralized productivity with transparency!
