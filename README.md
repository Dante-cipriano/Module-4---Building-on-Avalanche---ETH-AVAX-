# CellphonesShoppe Module 4 Assessment

# Overview

CellphonesShoppe is a smart contract that represents a shop selling different types of cellphones. The contract is based on the ERC20 standard and uses OpenZeppelin libraries. The owner of the contract can mint tokens, and users can transfer, redeem, and burn tokens.

# Transactions

### Minting

The owner can mint new tokens to any address.

```solidity
function mint(address _to, uint256 _amount) public onlyOwner
```

### Transferring

Users can transfer tokens to another address.

```solidity
function C_transfer(address _to, uint256 _amount) public
```

### Redeeming

Users can redeem their tokens for cellphones.

```solidity
function redeem(uint256 _amount) public
```

### Burning

Users can burn their tokens.

```solidity
function burn(uint256 _amount) public
```

### Checking Balance

Users can check their balance.

```solidity
function getBalance() external view returns (uint256)
```

### Cellphone Types

Users can view the types of cellphones available for sale.

```solidity
function typesofCellphones() external pure returns (string memory)
```

# Functions

- `mint(address _to, uint256 _amount)`: Mints `_amount` tokens to the address `_to`. Only callable by the owner.
- `C_transfer(address _to, uint256 _amount)`: Transfers `_amount` tokens to the address `_to`. Requires the sender to have enough balance.
- `redeem(uint256 _amount)`: Redeems tokens for cellphones. Requires the sender to have enough balance.
- `burn(uint256 _amount)`: Burns `_amount` tokens. Requires the sender to have enough balance.
- `getBalance()`: Returns the balance of the caller.
- `typesofCellphones()`: Returns a string listing the available types of cellphones and their prices.
- `decimals()`: Returns the number of decimals used for the token. Overrides the default to return `0`.

# Remix IDE

To deploy and interact with this contract, you can use [Remix IDE](https://remix.ethereum.org/). Follow these steps:

1. Open Remix IDE and create a new file named `CellphonesShoppe.sol`.
2. Copy and paste the contract code into the file.
3. Compile the contract using the Solidity compiler.
4. Deploy the contract by selecting the appropriate environment and clicking "Deploy".

# Owner

Dante Cipriano

# License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
