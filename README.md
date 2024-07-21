# ERC20 Token Implementation in Solidity

This Solidity contract provides a basic implementation of the ERC20 token standard, which is widely used for creating fungible tokens on the Ethereum blockchain. The contract includes functionalities such as minting, transferring, and burning tokens, along with maintaining the total supply and balances of token holders.
Features

  ERC20 Interface: Implements the IERC20 interface, which includes methods for getting the total supply, balance of a specific account, and transferring tokens.
   Ownership: Only the owner of the contract can mint new tokens, ensuring control over the token supply.
   Minting: The owner can generate new tokens to any address.
   Transferring Tokens: Allows token holders to transfer their tokens to other addresses.
   Burning Tokens: Token holders can reduce the total supply by burning (destroying) their tokens.

# Contract Components

   IERC20 Interface: Defines the standard functions for ERC20 tokens.
   ERC20 Contract: The main contract that implements the ERC20 standard.

# Key Variables and Functions

   ```owner```: The address of the contract owner, who is granted exclusive rights to mint new tokens.
  ```name, symbol, decimals```: Token metadata including its name, symbol, and decimals.
 ``` totalSupply:``` Represents the total token supply.
 ``` balanceOf:``` A mapping to keep track of each address's balance.
 ``` mint(uint _initialSupply):``` Allows the owner to mint new tokens.
  ```transfer(address recipient, uint amount):``` Enables token holders to transfer their tokens to another address.
  ```burn(uint amount):``` Allows token holders to burn their tokens, reducing the total supply.


# To interact with this contract:

   Deploy the Contract: Deploy the ERC20 contract to the Ethereum network, specifying the initial parameters like token name, symbol, and decimals.
   Mint Tokens: The owner can mint tokens by calling the mint function with the desired supply.
  Transfer Tokens: Token holders can transfer tokens to other addresses using the transfer method.
  Burn Tokens: Reduce the total token supply by burning tokens you own with the burn function.

# Development Environment

This contract is written for Solidity version 0.8.9. Ensure that your development environment is compatible with this Solidity version to avoid compilation errors.
License

This project is licensed under the MIT License.
