# SOLassessment
# MyToken - Simple Token Contract

This Solidity smart contract named `MyToken` is a basic implementation of a cryptocurrency token on the Ethereum blockchain. The contract manages a custom token referred to as "Cuzo" (token name: Cuzo, token abbreviation: CZO). The contract features functionalities to mint new tokens and burn existing tokens, keeping track of token balances and the total token supply.

# Contract Description

The `MyToken` contract provides the following features:

1. **Token Details**: The token details include the name "Cuzo," the abbreviation "CZO," and a total supply of tokens.
2. **Token Balances**: The contract maintains a mapping of addresses to store the token balances of individual addresses.
3. **Mint Function**: This function allows the creation of new tokens by increasing the total token supply and adding tokens to a specific address.
4. **Burn Function**: The burn function is the opposite of the mint function. It destroys tokens by reducing the total token supply and subtracting tokens from a specific address.
5. **Burn Safeguards**: The burn function includes conditional checks to ensure that the address balance has sufficient tokens to be burned.

# Functions

## `mint(address _address, uint _value)`

- Increases the total token supply by `_value`
- Adds the specified `_value` tokens to the balance of the `_address`

## `burn(address _address, uint _value)`

- Verifies if the `_address` holds enough tokens to be burned
- Reduces the total token supply by `_value`
- Decreases the `_address` balance by `_value` tokens

# Usage

You can deploy this contract to a supported Ethereum development network or testnet using a development environment like Remix or Truffle. After deployment, interact with the contract using the `mint` and `burn` functions to manage token creation and destruction.

## Note:

This contract is a basic example for educational purposes and should not be used in a production environment without thorough testing and auditing.

For more information on Solidity and Ethereum smart contracts, refer to the [Solidity Documentation](https://docs.soliditylang.org/).

