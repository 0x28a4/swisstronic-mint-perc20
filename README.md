# 📁 Example of PERC20 (Private ERC20)

This project demonstrates a basic PERC20 contract without comprehensive access-control logic. The main differences between ERC20 and PERC20 are protected balanceOf function and disabled Transfer and Approval events

## Build
To compile contracts, use the following command:
npm run compile

## Testing & Deployment
NOTE: tests are not compatible with hardhat network/ganache, so you have to start the Swisstronik local node or use public testnet

Create .env file from the example

cp example.env .env
Add PRIVATE_KEY in .env with the actual private key to interact with the network. If you're using other network than local testnet you also should replace URL in hardhat.config.ts

To run tests, use the following command:
npm run test

To deploy contracts, use check scripts/deploy.ts script and use the following command:
npm run deploy
