# Vision42Token Documentation

Vision42Token (V42) is an ERC-20 token built on the Ethereum blockchain.

---

## Features

- ERC20 standard token
- Mintable by the owner
- Transferable between users
- Compatible with Ethereum wallets

---

## Technologies Used

- Solidity
- Remix IDE
- OpenZeppelin Contracts
- MetaMask
- Sepolia Ethereum Testnet
- Etherscan

---

## Token Functions

- `transfer(address to, uint256 amount)`  
  Transfers tokens to another wallet.

- `balanceOf(address account)`  
  Returns the token balance of an account.

- `mint(address to, uint256 amount)`  
  Allows the contract owner to create new tokens.

- `approve(address spender, uint256 amount)`  
  Allows another address to spend tokens on behalf of the owner.

- `transferFrom(address from, address to, uint256 amount)`  
  Transfers tokens using an allowance.

- `transferOwnership(address newOwner)`  
  Change the owner of the token.

- `renounceOwnership()`  
  Remove the owner permanently (decentralizes token).

---

## How to Access and Interact with Vision42Token (V42)

### 1. Accessing the Token

**Add to MetaMask**

1. Copy the contract address:  
   `0x2cFC28FDC0fB80271BC36Ff05f74c0fB71a2A3a4`
2. Open MetaMask → **Import Tokens** → **Custom Token**.
3. Paste the contract address → the symbol (`V42`) and decimals (`18`) auto-fill.
4. Click **Add Token** → Now you can see your balance in MetaMask.

**Use Etherscan**

1. Go to the Sepolia Etherscan page for your token:  
   [Vision42Token on Sepolia](https://sepolia.etherscan.io/address/0x2cFC28FDC0fB80271BC36Ff05f74c0fB71a2A3a4)
2. View all transactions, holders, and token supply.
3. The **Contract** tab allows you to read/write functions directly.

**Use a Custom DApp (Web3 App)**

- Your front-end website (like the one you are building) can connect to MetaMask.
- Users interact directly with the blockchain through your app without using Etherscan.

---

### 2. Interactions Available

**a) Check Balance**

- Etherscan → `Read Contract` → `balanceOf(address)`
- MetaMask → automatically shows your balance
- Your DApp → shows the balance after connecting the wallet

**b) Transfer Tokens**

- Etherscan → `Write Contract` → `transfer(to, amount)`
- Your DApp → “Transfer” function/button
- MetaMask → use the token transfer interface

**c) Mint Tokens (Owner Only)**

- The owner (you, until renounced) can create new tokens:
  - Etherscan → `Write Contract` → `mint(to, amount)`
  - Your DApp → Mint section
- After calling `renounceOwnership()`, no one can mint more tokens.

**d) Ownership Functions**

- `transferOwnership(newOwner)` → Change the owner of the token
- `renounceOwnership()` → Remove the owner permanently (decentralizes token)

---

### 3. Notes for Users

- Only the owner can mint tokens. Regular users can only transfer and hold tokens.
- The token works on the Sepolia Testnet; it’s not real money yet.
- All transactions are public on the blockchain, but your personal identity is **not linked** to your wallet address unless revealed.
