# Real Estate NFT DApp

## Technology Stack & Tools

- Solidity (Writing Smart Contracts & Tests)
- Javascript (React & Testing)
- [Hardhat](https://hardhat.org/) (Development Framework)
- [Ethers.js](https://docs.ethers.io/v5/) (Blockchain Interaction)
- [React.js](https://reactjs.org/) (Frontend Framework)

## Requirements For Initial Setup
- Install [NodeJS](https://nodejs.org/en/)

## Setting Up
### 1. Clone/Download the Repository

### 2. Install Dependencies:
`$ npm install`

### 3. Run tests
`$ npx hardhat test`

### 4. Start Hardhat node
`$ npx hardhat node`

### 5. Run deployment script
In a separate terminal execute:
`$ npx hardhat run ./scripts/deploy.js --network localhost`

### 7. Start frontend
`$ npm run start`

## Sequence Diagram Explanation

The sequence diagram illustrates the flow of interactions between the Seller, Buyer, Inspector, Lender, Escrow Contract, and RealEstate Contract within the Real Estate NFT DApp. Here's a brief overview:

![Diagram](https://github.com/[username]/[reponame]/blob/main/millow/_docs/schemes/sequence.png?raw=true)

1. The Seller lists an NFT for sale on the Escrow Contract, specifying details such as the NFT ID, buyer, purchase price, and escrow amount.
2. The Buyer approves the sale and deposits earnest money, which is typically 50% of the purchase price.
3. An Inspector updates the inspection status of the property.
4. The Lender approves the sale and lends a portion of the purchase amount to the Buyer.
5. The Seller approves the sale and initiates the finalization process.
6. The Escrow Contract performs checks to ensure all parties have approved the sale, the inspection has passed, and the contract balance is sufficient.
7. If all checks pass, the NFT is transferred from the Escrow Contract to the Buyer, and the sale is finalized with funds transferred to the Seller.
8. If the sale is canceled, the Escrow Contract handles the cancellation and refunds the earnest money or sends it to the Seller based on the inspection status.

To view the sequence diagram, please refer to the following embedded image:


Please note that the actual sequence diagram image file should be generated from the provided PlantUML code and placed at the specified path for the iframe to work correctly.
