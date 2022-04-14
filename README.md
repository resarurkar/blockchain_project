# blockchain_project
blockchain project - Distribution of tokens to 10 different accounts using ERC20 Smart contract

#Distribution of tokens to 10 different metamask accounts using ERC20 smart contract

#In this project we are going to deploy a ERC20 smart contract on Ropsten test Network and using Node js we would be distributing it to 10 different netmask accounts.

To begin with we need to get 10 different accounts, in this case we already have the account details and hence we have updated the accounts.txt file with the same.

##Deployment
Pre-requisites 

We need to have node.js and Visual Studio Code for deployment.

Then we will have to check the node version which can be done as below
$bash
$node --version

Post that we need to install few modules to get the deployment running. That can be done using below commands

>npm install big-number
>npm install dotenv
>npm install web3
>npm install ethereumjs-tx

Once the modules are installed then we need to deploy the smart contract using Remix IDE. 

Copy the Deploymentcontract.sol code to Remix IDE and edit the token name as per the requirement.

Post doing changes now click on solidity compiler, select your account and click on compile.

Once done click Deploy button and select injected web3 and deploy the contract. This will automatically have MetaMask account to pop-up for authentication.

Select the Name of your token which you mentioned in the code and click on deploy. Open Metamask and confirm the tarnsaction.

##

Once this is done click on the transaction and copy the contract ID details and paste it in the environment file of VS code.

Go to Infura and create a project and copy the Project ID. Once that is done go back to VS code terminal.

Paste below details in environment file of VS Code 

•	MetaMask account address also know as  Owner_Address
•	Infura Token  The project code created in Infura.
•	A super-secret key  which can be found in MetaMask account
•	Contract Address  Deployed smart contract will have the contract ID.


Now from VS code terminal run below command:

node distribute.js

Once the code is executed 5% of the total tokens will be distributed to 10 different accounts of MetaMask.

After successful deployment we get the contract ID which needs to b
