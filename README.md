# Simple HTML Frontend for Fund Me

This is a simple HTML and JavaScript frontend for interacting with https://github.com/PCWCFA/fcc-hardhat-fund-me.

The project allows the interaction with the fund, balance, and withdraw functions of hardhat-fund-me.

# Setup & Configuration

## hardhat-fund-me-fcc

Run fcc-hardhat-fund-me on hardhat's localhost
yarn hardhat node to deploy the contracts on the localhost
Note the contract address

## Metamask

Import the localhost deployer account in Metamask

## html-fund-me-fcc

Run this project in VSCode
Install the Live Server plugin
Copy the contract address from the localhost net to constants.js's contractAddress.
Run the project using Live Server to bring up the HTML frontend in your default browser
Click on the Connect button to connect to Metamask.
Ensure you're connnecting to the deployer account.
Now you can fund, withdraw, and query the balance of the contract.

## Troubleshooting

Nonce error: Reset the account. This is because Metamask and localhost got out of sync as far as transaction counts.

RPC error at withdraw: Ensure that the account you imported from the locahost net is the first account. The contract only allows the owner/deployer account to withdraw.

# License

Distributed under the MIT License. See LICENSE.txt for more information.
