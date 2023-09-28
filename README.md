# Swisstronik Challenge #4


Here are your tasks:
Deploy an ERC20 token
Mint tokens
Transfer at least 1 of your ERC20 tokens to 0x16af037878a6cAce2Ea29d39A3757aC2F6F7aac1


# Introduction
### Token
```
Name   : ARAPZZ
Symbol : ARPZ
```
### Smart Contract
```
0xcCeceeeCa51587634904C06C00cf26b3dB87126E
```
### Function Mint 100 Tokens
```
function mint100tokens() public {
    _mint(msg.sender, 100*10**18);
}

```
### Function Transfer 10 Tokens
```
  const replace_functionName = "transfer";
  const replace_functionArgs = ["0x16af037878a6cAce2Ea29d39A3757aC2F6F7aac1", "10"];
  const transaction = await sendShieldedTransaction(signer, replace_contractAddress, contract.interface.encodeFunctionData(replace_functionName, replace_functionArgs), 0);
```

### Explorer Deploy
```
https://explorer-evm.testnet.swisstronik.com/tx/0x354407c1124001f9673c51e81837c4d6412bf2c1760f8167573560ba48337b21
```
### Explorer Minting
```
https://explorer-evm.testnet.swisstronik.com/tx/0x0a2335ca658eeb62f04e91ea562ce7848ee9255c70cfd1227021e92fd4fc7b17
```
### Explorer Transfer
```
https://explorer-evm.testnet.swisstronik.com/tx/0x9c0ffd612cb2e32a1c547815ebdc396b6bad63f0eb86b215a67c8ece7e866c8a
```

### Log Deploy
 <p align="center">
 <img height="auto" height="auto" src="https://raw.githubusercontent.com/arapzz/images/main/swiss/Screenshot%202023-09-28%20082051.png">
 </p>

### Log Transfer 
 <p align="center">
 <img height="auto" height="auto" src="https://raw.githubusercontent.com/arapzz/images/main/swiss/Screenshot%202023-09-28%20082221.png">
 </p>

### Log Balance 0x16af037878a6cAce2Ea29d39A3757aC2F6F7aac1
 <p align="center">
 <img height="auto" height="auto" src="https://raw.githubusercontent.com/arapzz/images/main/swiss/Screenshot%202023-09-28%20082304.png">
 </p>
     
# Usage
```
npm install --save-dev hardhat
npx hardhat
npm install --save-dev @nomicfoundation/hardhat-toolbox
npm install @openzeppelin/contracts
npm install @swisstronik/swisstronik.js
npx hardhat run scripts/deploy.js
npx hardhat run scripts/mint.js
npx hardhat run scripts/transfer.js
```
