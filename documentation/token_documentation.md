# Vision42Token Documentation

Vision42Token (V42) is an ERC-20 token built on the Ethereum blockchain.

## Features

- ERC20 standard token
- Mintable by the owner
- Transferable between users
- Compatible with Ethereum wallets

## Technologies Used

- Solidity
- Remix IDE
- OpenZeppelin Contracts
- MetaMask
- Sepolia Ethereum Testnet
- Etherscan

## Token Functions

transfer(address to, uint256 amount)
Transfers tokens to another wallet.

balanceOf(address account)
Returns the token balance of an account.

mint(address to, uint256 amount)
Allows the contract owner to create new tokens.

approve(address spender, uint256 amount)
Allows another address to spend tokens on behalf of the owner.

transferFrom(address from, address to, uint256 amount)
Transfers tokens using an allowance.