# NFT RUN
A classic game similar to Chrome Dino where you can claim game rewards in the form of NFTs &amp; Game Tokens.


## Technology Stack & Dependencies

- Solidity (Writing Smart Contract)
- HTML, Css, Javascript & Bootstrap For the website
- [Alchemy](https://www.alchemy.com/) Account on Alchemy as a node provider
- [NodeJS](https://nodejs.org/en/) To install Dependencies
- [Hardhat](https://hardhat.org/) Ethereum development environment
- [Ethers.js](https://docs.ethers.io/v5/) To interact with the blockchain

### 1. Clone/Download the Repository

### 2. Install Dependencies:
```
$ cd contracts
$ npm install
```

### 3. Deploy NFT collection to Polygon Mumbai testnet
- Setup your env file with both private key and mumbai RPC 
```
MUMBAI_RPC=https://polygon-mumbai.g.alchemy.com/v2/...
PRIVATE_KEY=...
```

```
$  npx hardhat run scripts/deployNFTCollection.js --network mumbai
```

### 4. Deploy Run token to Polygon Mumbai testnet
- Setup your env file with both private key and mumbai RPC 
```
$  npx hardhat run scripts/deployRunToken.js --network mumbai
```

### 5. Update the smart contract addresses in blockchain.js file
- These will be displayed in the terminal after running the previous two commands successfully
```
const runTokenContractAddress = "...";
const nftContractAddress = "...";
```
