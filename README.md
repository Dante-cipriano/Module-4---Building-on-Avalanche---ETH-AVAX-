# DotaPoints Smart Contract

## Overview
DotaPoints is an ERC20-compliant token contract built on the Ethereum blockchain. It facilitates the creation, transfer, and redemption of "DOTA" tokens, which can be used to acquire in-game items related to Dota 2. The contract also includes functionalities for minting new tokens, burning tokens, and managing ownership.

# Functions

# ERC20 Standard Functions
  totalSupply: Returns the total supply of Dota Points tokens.
  balanceOf: Returns the balance of tokens for a given address.
  transfer: Transfers tokens from the sender's address to a recipient.
  allowance: Returns the amount of tokens that the spender is allowed to spend on behalf of the owner.
  approve: Allows the spender to withdraw tokens from the owner's account multiple times, up to the approved amount.
  transferFrom: Transfers tokens from one address to another, given approval from the sender.

# Additional Functions
 mint: Allows the contract owner to mint (create) new Dota Points tokens and allocate them to a specified account.
 redeem: Enables users to redeem predefined in-game items using their Dota Points tokens. Tokens are transferred to the contract owner upon redemption.
 burn: Allows users to burn (destroy) their Dota Points tokens, reducing the total supply.
 getAvailableItems: Returns an array of available in-game items that can be redeemed using Dota Points tokens.
 getRedeemed: Returns a boolean array indicating which in-game items have been redeemed by a specific user.

# Owner
Cipriano Jr. Dante R. 

# License
This project is licensed under the MIT License. See [LICENSE](./LICENSE) for more details.
