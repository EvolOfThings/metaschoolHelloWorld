# [Metaschool](https://metaschool.so/) - Writing a Smart contract in Solidity

Notes 

```sh 
 A smart contract mainly has states, functions and events. 

* States => variables, token and NFTs whose state we want to maintain in the SC.
* Functions => functions are used to read, write or change the states
* Events => events are activated based on a transformation in a state, a call to a function etc.
```



> Ether.js is a library helps us interact with blockchain, we can deploy, fetch SC and call their functions.
Hardhat ethers is a plugin that gives access to ethers.js library.deploy.js script tells how the SC should be deployed.
Contract factory is like template for a SC, that lets us create a new instances of the contract. The new instance of SC is stored in a variable (here hw is that variable) and it’s a copy of our contract but lives in the Ethereum blockchain at a specific address.

> Interact.js script is basically changing or interacting with the SC that’s already deployed to the chain.
With help of hardhat ethers, we get contract’s ABI(Application Binary Interface) and other info from a JSON file. ABI is a set of instructions for interacting with the contract, and it’s needed to create an instance of the contract.

> Once we have all the functions from ethers, we initiate main function. Here we make a get the message and await it. Next we call update function from the SC and write new message, then wait til the transaction takes place on the chain. And then we log on the console to check if the new message is saved not he chain. We can check goerli etherscan by looking up the contract address to see the transaction.