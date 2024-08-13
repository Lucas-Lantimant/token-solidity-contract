# Token Contract

## Overview

This Solidity smart contract implements a basic ERC-20 token with fundamental functionalities. The token is named "TOKEN COIN" with the symbol "TKN" and uses 18 decimal places. It provides essential operations such as transferring tokens, approving allowances, and querying balances and allowances.

## Contract Details

- **Symbol**: TKN
- **Name**: TOKEN COIN
- **Decimals**: 18
- **Total Supply**: 1,000,000 TKN

## Functions

### `totalSupply()`
Returns the total supply of the token.

### `balanceOf(address tokenOwner)`
Returns the balance of a specific address.

### `transfer(address to, uint256 tokens)`
Transfers tokens from the caller's account to another account. Requires that the caller has sufficient balance.

### `approve(address spender, uint256 tokens)`
Allows a spender to withdraw from the caller's account multiple times, up to the specified amount. This is part of the ERC-20 approval mechanism.

### `allowance(address tokenOwner, address spender)`
Returns the amount of tokens that a spender is allowed to withdraw from a token owner's account.

### `transferFrom(address from, address to, uint256 tokens)`
Transfers tokens from one account to another using an allowance mechanism. Requires that the caller is approved to spend the tokens and that the from account has sufficient balance.

## Events

- **Transfer**: Emitted when tokens are transferred from one account to another.
- **Approval**: Emitted when an account approves a spender to withdraw tokens.

## Constructor

The constructor sets the total supply of tokens and assigns the entire supply to the account that deploys the contract. It also emits a Transfer event for the initial supply.

---

This contract is a straightforward implementation of an ERC-20 token and provides a foundation for building more complex token systems.

## License

This project is licensed under the `MIT License` - see the LICENSE file for details.