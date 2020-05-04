# SmartMint-BondBill ERC-721 token lending platform

## 💡 SmartMint-BondBills-Collateralized Description 💡
SmartMint-BondBills-Collateralized is Ethereum Smart Contract that allows lending ERC-721 Smart Contracts (NFT)
and gain interest from it. On the other hand it allows to borrow same NFT's that are
set for lending by paying collateral to LEND721 which handles the lend process.

Current stage: **alpha**.

## 🏹 Deployed client dApps on Netlify as example concept of this contract use case in other projects 🏹:

- Mainnet: [https://lend721.app](https://lend721.app)
- Rinkeby: [https://rinkeby.lend721.app](https://rinkeby.lend721.app)

## 🏠 Current Betatesting Smart Contract addresses across Ethereum networks in other use cases 🏠
- Mainnet: [0xA133541435cAeB964f572132acd8FEAC3Ed1D80B](https://etherscan.io/address/0xA133541435cAeB964f572132acd8FEAC3Ed1D80B)
- Rinkeby: [0x1762fd547d6C286a174dD62b6A6fACFAc064A0A0](https://rinkeby.etherscan.io/address/0x1762fd547d6C286a174dD62b6A6fACFAc064A0A0)

```
Note: Smart Contract calls are proxied to main Smart Contract so calls destination is the Proxy Smart Contract itself.
```

## ✅ To do
- [x] Client dApp: show lent data
- [x] Client dApp: show borrowed data
- [x] Client dApp borrower: call DAI approve method
- [x] Client dApp borrower: call borrow method
- [x] Client dApp lender: call ERC-721 approve method
- [x] Client dApp lender: call ERC-721 lend set method
- [x] Set duration for lendings
- [x] Deploy Smart Contract to mainnet
- [x] Verify Smart Contract in mainnet Etherscan
- [x] Put lenders addresses with lent tokens somwehere outside of smart contract (UX improvement) – (note: solved with thegraph.com)
- [ ] Show message when collateral was already taken on expired lend
- [ ] Show success or error messages on each transaction
- [ ] Email reminders for borrower or lender
- [ ] Allow edit lend

## 🧩 Deploy to The Graph 

Run from `.thegraph`:
```
yarn subgraph:prepare
yarn subgraph:codegen
yarn subgraph:deploy
```

More info – [thegraph.com/docs/deploy-a-subgraph](https://thegraph.com/docs/deploy-a-subgraph).

