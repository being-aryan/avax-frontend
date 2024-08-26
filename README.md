# MyToken Interface

This project combines a Next.js front-end with a Hardhat development environment for Ethereum smart contracts.

## Prerequisites

- Node.js and npm installed on your computer
- MetaMask extension installed in your browser

## Getting Started

### 1. Install Dependencies in Terminal 1

Inside the project directory, install the required npm packages:

```bash
npm install
```

### 2. Start the Hardhat Local Node in Terminal 2

Open a new terminal and start the Hardhat local blockchain node:

```bash
npx hardhat node
```

This will start a local Ethereum network for development.

### 3. Deploy the Smart Contracts Terminal 3

In another terminal, deploy the smart contracts to the local network:

```bash
npx hardhat run --network localhost scripts/deploy.js
```

This will compile and deploy your smart contracts to the local Hardhat network.

### 4. Launch the Front-End

Back in the first terminal, start the Next.js development server:

```bash
npm run dev
```

This will launch the front-end application, typically accessible at `http://localhost:3000/`.

## Connecting MetaMask

To interact with the deployed contracts, you need to connect MetaMask to the local Hardhat network:

1. Open MetaMask and click on the network dropdown at the top.
2. Select "Custom RPC".
3. Enter the following details:
    - **Network Name**: Localhost 8545
    - **New RPC URL**: http://localhost:8545
    - **Chain ID**: 1337 (default Hardhat network ID)
4. Save the network.

Then, import one of the generated accounts from the Hardhat node into MetaMask using the private keys displayed in the Hardhat terminal.

## Common Issues

- **Dependencies Not Installed**: Make sure you run `npm install` inside the project directory.
- **Error: "Internal JSON-RPC error"**: Ensure that your MetaMask is connected to the correct network and the contract address is correct.
## Authors
aryan09
## License

[MIT License](./LICENSE)
