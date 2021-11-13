# Brownie Simple Storage

Basic storage Solidity smart contract using [Brownie](https://eth-brownie.readthedocs.io/en/stable/) framework.

Following Patrick Collins 'Solidity, Blockchain, and Smart Contract Course – Beginner to Expert Python Tutorial' course on freeCodeCamp

## 

Install Brownie : 
```bash
pip install eth-brownie
```

Run tests : 
```bash
brownie run test
```

Deploy to local network (brownie will use ganache to deploy a dev network) : 
```bash
brownie run scripts/deploy.py
```

Deploy to a testnet :

1. Export your test account PRIVATE_KEY in a .env file
2. Setup a project on [Infura](https://infura.io/) on the testnet you want to deploy the contract on
3. Export the Infura project ID in the .env file as WEB3_INFURA_PROJECT_ID
4. Run : 
```bash
brownie run scripts/deploy.py --network [TESTNET NAME]
```

Interact with the deployed contract on a testnet : 
```bash
brownie run scripts/read_value.py --network [TESTNET NAME]
```
