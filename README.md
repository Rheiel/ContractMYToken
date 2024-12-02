# **MyToken Smart Contract (ERC-20)**

### **Overview**
**MyToken** is an ERC-20 token that includes functionalities for minting, transferring, and burning tokens. It integrates OpenZeppelin’s libraries for secure and standard token management. This smart contract ensures owner-only minting while allowing all users to transfer and burn tokens.

---

### **Features**
- **Minting**: Only the contract owner can mint tokens.
- **Transferring**: Any user can transfer tokens.
- **Burning**: Any user can burn their tokens.
- **Ownership Management**: Secure ownership control using OpenZeppelin’s `Ownable` contract.

---

### **Functions Overview**

#### 1. **Mint Tokens**
```solidity
function mint(address to, uint256 amount) public onlyOwner
