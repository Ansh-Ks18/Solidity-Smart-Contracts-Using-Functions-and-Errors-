# SimpleBank Smart Contract

## Project Title
SimpleBank Smart Contract

## Simple Overview
A basic Ethereum smart contract that implements a simple banking system with deposit, withdrawal, and transfer functionalities.

## Description
The SimpleBank smart contract is designed to manage a simple banking system on the Ethereum blockchain. Users can deposit Ether into their accounts, withdraw Ether from their accounts, and transfer Ether to other accounts. This contract includes events to log these actions for transparency and ease of tracking.

## Getting Started

### Installing

#### How/where to download your program
You can copy the contract code from the `Contract SimpleBank` file in this repository.

#### Any modifications needed to be made to files/folders
No modifications are necessary. You can use the contract as is, but you are free to modify the code as per your requirements.

### Executing program

#### How to run the program

1. **Set Up Your Development Environment**:
    - Use [Remix IDE](https://remix.ethereum.org/) or any other Solidity development environment.
    
2. **Copy the Contract Code**:
    - Copy the code from `Contract SimpleBank`.

3. **Compile the Contract**:
    - Paste the copied code into your Solidity file in Remix IDE.
    - Click on the "Solidity Compiler" tab and compile the contract.

4. **Deploy the Contract**:
    - Go to the "Deploy & Run Transactions" tab.
    - Select the desired environment (e.g., JavaScript VM, Injected Web3 for MetaMask).
    - Click "Deploy" to deploy the contract.

#### Step-by-step bullets

- **Deposit Funds**:
    ```solidity
    simpleBankInstance.deposit({value: web3.utils.toWei("1", "ether")});
    ```
    This command deposits 1 Ether into the sender's account.

- **Withdraw Funds**:
    ```solidity
    simpleBankInstance.withdraw(web3.utils.toWei("0.5", "ether"));
    ```
    This command withdraws 0.5 Ether from the sender's account, provided the account has sufficient balance.

- **Transfer Funds**:
    ```solidity
    simpleBankInstance.transfer("0xRecipientAddressHere", web3.utils.toWei("0.3", "ether"));
    ```
    This command transfers 0.3 Ether from the sender's account to the specified recipient address.

### Help
For common problems or issues, ensure:

- You have sufficient balance for withdrawal and transfer functions.
- The addresses used in functions are correct and valid.

If the contract fails to deploy, verify your Solidity version and ensure compatibility with the compiler settings.

## Authors

- **Your Name** - @AnshuKumar

## License
This project is licensed under the MIT License - see the LICENSE.md file for details.

---

For more information, please refer to the [Solidity Documentation](https://docs.soliditylang.org/).
