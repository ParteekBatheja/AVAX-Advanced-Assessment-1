# AVAX Advanced Assessment - 1

Creating an EVM Subnet and deploying ERC-20 and Vault smart contracts on Avalanche using Remix.

## Description

This project provides a comprehensive guide to setting up an EVM Subnet on Avalanche and deploying essential smart contracts: an ERC-20 token contract and a Vault contract. These contracts serve as foundational building blocks for a DeFi Kingdom clone, enabling developers to explore the exciting world of decentralized finance and take their first steps towards building their own DeFi empire.

## Getting Started

### Installing

1. **Install Avalanche CLI:**
   Follow the instructions in the [Avalanche CLI documentation](https://docs.avax.network/build/tools/avalanche-cli) to install the CLI tool.

### Executing Program

To create an EVM Subnet and deploy the smart contracts, follow these steps:

1. **Create a new subnet:**

    ```bash
    avalanche subnet create mySubnet
    ```

2. **Select the EVM Subnet option and configure it:**
   Follow the prompts to set up your EVM Subnet, including specifying the ChainId and token symbol.

3. **Deploy the subnet:**

    ```bash
    avalanche subnet deploy mySubnet
    ```

4. **Connect to MetaMask:**
   Follow the instructions provided in the Avalanche CLI output to connect your subnet to MetaMask.

5. **Open Remix IDE:**
   Visit [Remix IDE](https://remix.ethereum.org/).

6. **Deploy ERC-20 Token Contract:**

    - **Create a new file in Remix named `ERC20.sol`.**
    - **Copy and paste the code from the [ERC20.sol](ERC20.sol) file in this repository into your new file in Remix.**
    - **Compile the contract.**
    - **Deploy the contract using the Injected Web3 environment (ensure MetaMask is connected to your EVM Subnet).**
    - **Note down the deployed contract address of the ERC-20 token, as this will be required for deploying the Vault contract.**

7. **Deploy Vault Contract:**

    - **Create a new file in Remix named `Vault.sol`.**
    - **Copy and paste the code from the [Vault.sol](Vault.sol) file in this repository into your new file in Remix.**
    - **In the constructor of `Vault.sol`, provide the address of the deployed ERC-20 token contract.**
    - **Compile the contract.**
    - **Deploy the contract using the Injected Web3 environment (ensure MetaMask is connected to your EVM Subnet).**

### Interacting with the Contracts

Once deployed, developers can interact with the contracts directly in Remix:

- **ERC-20 Token Contract (ERC20.sol):** Manage token minting, transfers, and burning.
- **Vault Contract (Vault.sol):** Handle deposits and withdrawals of tokens.

### Modifications

No modifications are required for basic functionality. If desired, you can customize or expand the contracts' functionality by modifying the code accordingly.

## Authors

Parteek Batheja  
[@ParteekBatheja](https://github.com/ParteekBatheja)

## License

This project is licensed under the MIT License. See the [LICENSE.md](LICENSE.md) file for details.
