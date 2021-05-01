# Solidity and Hardhat project startup wired to BSC

`npm init --yes `

### install packages

`npm install --save-dev hardhat`

`npx hardhat`

`npm install --save-dev @nomiclabs/hardhat-waffle ethereum-waffle chai @nomiclabs/hardhat-ethers ethers`

- Choose -> Create a sample project

### Compile Contract

`npx hardhat compile`

### Run Tests

`npx hardhat test`

### Deploy Contract to BSC (testnet) or (mainnet)

`npm install --save-dev @nomiclabs/hardhat-etherscan`

`npx hardhat run --network testnet scripts/deploy.js`
or
`npx hardhat run --network mainnet scripts/deploy.js`

- Check Deployment on here: https://bscscan.com/ or https://testnet.bscscan.com/ (mainnet)

### Verify Contract on BSC

- Go to register and get API key: https://bscscan.com/myapikey
- Add API_KEY to `hardhat.config.js`

`$ npx hardhat verify --network testnet pasteYourContractAdressHere`

- Optionally (Constructor Argument)

`npx buidler verify --network testnet DEPLOYED_CONTRACT_ADDRESS "Constructor argument 1"`


