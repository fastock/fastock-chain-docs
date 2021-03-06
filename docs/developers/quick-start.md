# Quick Start for Testnet
## Metamask
Connect your Metamask wallet with faStock-Chain Testnet.
## Adding a custom network for faStock-Chain Testnet
Open the Metamask extension on your browser, you may have to log in to your Metamask account if you are not already. Then click the top right circle and go to Settings > Networks. Press the Add Network button and fill the form as shown below with your application ChainID.

Config your Metamask with following data   

- NetWork Name: faStock-Chain Testnet
- RPC URL: [Rest Address](blockchainDetail/rpc.html#rest-endpoint)
- Chain ID: 65
- Currency Symbol: OKT

![avatar](../img/metamask-01.jpg)

Use fastock-chain-cli to view accounts:

`fastock-chain-cli keys show $keyname`

Use fastock-chain-cli to export the ethereum style private key:

`fastock-chain-cli keys unsafe-export-eth-key $keyname`

import private key into the metamask wallet:

![avatar](../img/metamask-01-2.png)

The relationship between fastock-chain address and 0x address:

- The balance of the address starting with fastock-chain is equal to the balance of the address starting with 0x
- The balance of the address starting with fastock-chain can only be queried through fastock-chain-cli
- The balance of the 0x address can be queried through the evm rpc interface, or through the fastock-chain-cli

-------------------------------------------------------------
-------------------------------------------------------------
## Remix
Set up a Remix faStock-Chain Testnet development environment.    
Remix is an in-browser IDE for Solidity smart contracts. In this guide, we will learn how to deploy a contract to a running faStock-Chain Testnet through Remix and interact with it.   
### 1. Connect faStock-Chain account to Remix
Go to [Remix](http://remix.ethereum.org/). There are some contracts in the File Explorer. Select any of these contracts. In this example, we use `Storage.sol`. On the left-most bar, select the Solidity Compiler and compile the contract.


![avatar](../img/metamask-02.png)

Next, select the `Deploy and Run` option. Select `injected web3` as the environment. This will open a metamask popup for you to confirm connecting your Metamask to Remix. Hit confirm.

You should see your account show up in the left-hand panel.

![avatar](../img/metamask-03.png)


### 2. Deploy and Interact
Now that your account is connected, you are able to deploy the contract. Press the Deploy button. A metamask pop-up will appear asking you to confirm. Confirm the transaction   

Once the contract has been successfully deployed, you will see it show up in the Deployed Contracts section in the left-hand side, as well as a green check in the Remix console showing the transaction details.   

![avatar](../img/metamask-04.png)


Now, you are able to interact with the contract through Remix. For Storage.sol, input 1000 and click `store`. This will open a Metamask pop-up asking you to confirm. Confirm the transaction. Then, click `retrieve` to get the number, which should be 1000.

![avatar](../img/metamask-05.png)


-------------------------------------------------------------
-------------------------------------------------------------
## Claim test tokens
Please refer to [Faucet](https://www.fastock.com/drawdex)
