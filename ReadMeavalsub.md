Vault README
This repository contains a simple implementation of a Solidity smart contract named Vault that acts as a basic vault for managing deposits and withdrawals of an ERC-20 token. The contract follows the ERC-20 standard and includes functionality for depositing and withdrawing funds, as well as tracking user balances and total supply.

Smart Contract Details
SPDX-License-Identifier
This smart contract is licensed under the MIT License. Please refer to the LICENSE file for more details.

Solidity Version
The contract is written in Solidity and requires version 0.8.17 or higher.

ERC-20 Interface
The contract implements the ERC-20 interface through the IERC20 interface. The standard ERC-20 functions are present, including totalSupply, balanceOf, transfer, allowance, approve, transferFrom, as well as the associated Transfer and Approval events.

Vault Contract
The main contract is named Vault, and it is designed to hold and manage a specific ERC-20 token. The token is specified during contract deployment and is immutable once set.

State Variables
token: An immutable reference to the ERC-20 token managed by the vault.
totalSupply: The total supply of shares in the vault.
balanceOf: A mapping that keeps track of the balance of shares for each account.
Constructor
The constructor initializes the vault with a specific ERC-20 token.

Deposit Function
The deposit function allows users to deposit ERC-20 tokens into the vault. The number of shares issued to the user is determined based on the current total supply and the amount being deposited.

Withdraw Function
The withdraw function allows users to withdraw their shares from the vault in exchange for the corresponding amount of ERC-20 tokens. The number of shares to burn is determined based on the requested withdrawal amount and the current total supply.

Usage
To use this contract, deploy it to a compatible Ethereum network, passing the address of the ERC-20 token to be managed by the vault. Users can then interact with the contract by depositing and withdrawing tokens.

Please ensure you understand the risks associated with interacting with smart contracts on the Ethereum blockchain.

License
This project is licensed under the terms of the MIT license. See the LICENSE file for details.
