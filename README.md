# Assesment-3.3
# Project Title
write a smart contract to create your own ERC20 token and deploy it using HardHat or Remix.
## Description
This project involves the creation of a Solidity smart contract for an ERC20 token named "MyToken" (symbol: "MT"). The contract includes functionalities for minting new tokens and burning existing ones. The contract owner has the exclusive right to mint new tokens, while any token holder can burn their tokens. The project demonstrates the application of Solidity for creating and managing a custom ERC20 token using OpenZeppelin's ERC20 implementation.


## Getting Started

Contract Details:

Imports:

The contract imports the ERC20 contract from the OpenZeppelin library, which provides a standard implementation of the ERC20 token standard.

State Variables:

owner: Stores the address of the contract owner (the account that deploys the contract).

Constructor:

The constructor sets the deployer as the contract owner and mints an initial supply of 1,000,000 tokens to the owner's address. The initial supply is adjusted for the token's decimals.

Mint Function:

mint(address to, uint256 amount): Allows the contract owner to mint new tokens and allocate them to a specified address. The function includes a require statement to ensure that only the owner can call this function.

Burn Function:

burn(uint256 amount): Allows any token holder to burn (destroy) a specified amount of their own tokens. The function calls the _burn method from the ERC20 implementation to reduce the total supply and the caller's balance

### Installing

In this evaluation, we will  use Remix IDE. Remix IDE is an online tool that makes creating, assembling, implementing, and testing Ethereum blockchain smart contracts easier.

use remix ide of version 0.8.18 to run code properly

### Executing program
Execution Program:
Step 1: Setup and Compilation

Open Remix IDE (https://remix.ethereum.org/).

Create a new file named MyToken.sol.

Copy and paste the provided Solidity code into the new file.

Compile the contract using the Solidity compiler version 0.8.20.

Step 2: Deploy the Contract

In Remix, go to the "Deploy & Run Transactions" tab.

Select the MyToken contract and deploy it.

Note the deployed contract address and the initial supply of tokens minted to the owner's address.

Step 3: Interact with the Contract

Mint Tokens:

Call the mint function with the recipient's address and the amount to mint.

Example: myToken.mint("0xRecipientAddress", 1000 * 10 ** myToken.decimals())

Ensure you are using the owner’s address to perform this action.

Burn Tokens:

Call the burn function with the amount of tokens to burn.

Example: myToken.burn(500 * 10 ** myToken.decimals())

Any token holder can perform this action.

Check Balances:

Use the standard ERC20 balanceOf function to check the token balances of any address.

Example: myToken.balanceOf("0xSomeAddress")


## Help

OpenZeppelin Library: The contract relies on the OpenZeppelin library, so make sure to install and import it correctly
use remix IDE of version 0.8.20;

## Authors

Contributors names and contact info

Sarvagya pathak 

 adittyapathak8081@gmail.com


## License

This project is licensed under the Sarvagya pathak  
