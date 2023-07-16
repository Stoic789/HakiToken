
# Haki Token

Haki is a decentralized digital token built on the Ethereum blockchain. It leverages smart contracts to provide a reliable and transparent ecosystem for secure and efficient transactions. This repository contains the Solidity code for the Haki token contract.

## Features

- ERC20 Compatibility: Haki adheres to the widely adopted ERC20 standard, allowing for seamless integration with other Ethereum-based tokens and platforms.
- Minting and Burning: The contract owner has the exclusive authority to mint new tokens, ensuring token supply control and stability. Additionally, tokens can be burned to reduce the supply.
- Secure and Efficient Transactions: Haki utilizes the Ethereum network for fast and cost-effective transfers.

## Functionalities

### Minting Tokens

The contract owner, defined during deployment, has the ability to mint new tokens. This feature is useful for expanding the token supply. The `mint` function allows the owner to mint a specified amount of tokens and assign them to a particular address.

### Burning Tokens

The burning feature enables the reduction of the token supply. Tokens can be burned to maintain control over the circulating supply. The `burn` function allows any token holder to burn their own tokens, reducing the total supply accordingly.

### Secure Transactions

The `transfer` function facilitates secure and efficient token transfers between addresses. By calling this function, token holders can send tokens from their own account to another address. The transfer is executed securely, ensuring the integrity of the transaction.

## Contract Owner and `onlyOwner` Modifier

The contract owner is the address that initially deploys the contract. Only the contract owner has access to certain functions, such as minting tokens. The `onlyOwner` modifier is used in the `mint` function to restrict access to only the contract owner. This ensures that only the authorized owner can mint new tokens, providing control and security over the token supply.

## Input Types

- `address`: Ethereum address of an account.
- `uint256`: Unsigned integer representing a numerical value, such as the amount of tokens to be minted or burned.

## Usage

1. Install dependencies:
   - Solidity Compiler: ^0.8.9
   - OpenZeppelin Contracts: v4.3.1

2. Deploy the contract:
   - Set the contract owner during deployment.

3. Interact with the contract:
   - Mint new tokens: The contract owner can call the `mint` function, providing the recipient's address and the amount of tokens to be minted.
   - Burn tokens: Any token holder can call the `burn` function to burn a specified amount of their own tokens.
   - Transfer tokens: Users can call the `transfer` function to send tokens from their account to another address.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.

## Resources

- [Solidity Documentation](https://docs.soliditylang.org/)
- [OpenZeppelin Contracts](https://github.com/OpenZeppelin/openzeppelin-contracts)
