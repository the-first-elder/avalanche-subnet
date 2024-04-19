# Vault Contract

## Overview

This repository contains the smart contract code for a `Vault` contract, which is designed to manage deposits and withdrawals of ERC20 tokens in a decentralized finance (DeFi) context. The `Vault` contract allows users to deposit ERC20 tokens into the vault and receive shares in return, which can be redeemed for the underlying tokens at any time. This mechanism is commonly used in DeFi platforms to provide liquidity and yield farming opportunities.

## Features

- **Deposit**: Users can deposit ERC20 tokens into the vault. In return, they receive shares that represent their proportionate ownership of the vault's total assets.
- **Withdraw**: Users can redeem their shares for the underlying ERC20 tokens. The amount of tokens received is proportional to the number of shares they hold.
- **ERC20 Compatibility**: The vault is compatible with any ERC20 token, making it versatile for various use cases.

## Installation

To interact with this contract, you will need a Solidity compiler (solc) and a development environment like Truffle or Hardhat. Ensure you have Node.js and npm installed, then:

1. Clone this repository. 
2. Run `forge install` to install dependencies.
3. Compile the contracts using `forge compile`

## Usage

### Deploying the Contract

To deploy the `Vault` contract, you will need to have a development blockchain running (e.g., Ganache for local testing) or access to a testnet/mainnet. Use the deployment scripts provided in the `scripts` directory or deploy manually using your preferred development environment.

### Interacting with the Contract

Once deployed, you can interact with the `Vault` contract using web3.js, ethers.js, or any other Ethereum library. Here are some basic interactions:

- **Deposit**: To deposit tokens into the vault, call the `deposit` function with the amount of tokens you wish to deposit. Ensure you have approved the vault contract to spend your tokens.
- **Withdraw**: To withdraw your shares and receive the underlying tokens, call the `withdraw` function with the number of shares you wish to redeem.


## Security

This contract is provided as-is and should be thoroughly audited before use in production environments. Always follow best practices for smart contract development and security.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.