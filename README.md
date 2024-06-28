## Overview
'MyToken' is a simple Ethereum-based token contract implemented in Solidity. This contract allows you to mint and burn tokens, keeping track of balances and total supply. Below are the key features and functionalities of the contract.

## Features

1. **Token Details**
    - **Token Name:** ASHU
    - **Token Abbreviation:** ASH
    - **Total Supply:** Dynamically updated based on minting and burning operations.

2. **Balances Mapping**
     Maintains a mapping of addresses to their respective token balances.

3. **Mint Function**
     Adds a specified number of tokens to an address's balance and increases the total supply.

4. **Burn Function**
     Removes a specified number of tokens from an address's balance and decreases the total supply, provided the address has enough tokens.

## Contract Details

### State Variables
- 'tokenName' (string): The name of the token.
- 'tokenAbbrv' (string): The abbreviation of the token.
- 'totalSupply' (uint): The total supply of the token.
- 'balances' (mapping(address => uint)): A mapping from addresses to their token balances.

### Functions

#### `mint`
(function mint(address _address, uint _value) public)

**Description:** Mints '_value' tokens to the '_address' and updates the total supply.
  **Parameters:**
   '_address' (address): The address to which the tokens will be minted.
   '_value' (uint): The number of tokens to mint.

#### `burn`
(function burn(address _address, uint _value) public)
 **Description:** Burns `_value` tokens from the '_address' if the address has enough balance, and updates the total supply.
  **Parameters:**
   '_address' (address): The address from which the tokens will be burned.
   '_value' (uint): The number of tokens to burn.

  **Condition:** The function checks if the balance of `_address` is greater than or equal to `_value` before burning the tokens.



## Author

Ayushi Bisht
