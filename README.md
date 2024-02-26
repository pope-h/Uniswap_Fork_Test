# Uniswap Interaction README

/*
This repository contains scripts to interact with Uniswap decentralized exchange using Hardhat and ethers.js.
*/

// Setup

/*
1. Clone this repository:

git clone <repository-url>

2. Navigate to the project directory:

cd <project-directory>

3. Install dependencies:

npm install
*/

// Usage

/*
### 1. Swapping USDC for DAI

To swap USDC for DAI, run the `swap.js` script:

npx hardhat run scripts/swap.js

This script performs the following steps:
- Impersonates a specific account holding USDC.
- Approves the Uniswap router to spend USDC on behalf of the account.
- Swaps USDC for DAI using Uniswap's `swapExactTokensForTokensSupportingFeeOnTransferTokens` function.
- Prints account balances before and after the swap.

### 2. Adding Liquidity to Uniswap Pool

To add liquidity to a Uniswap pool with USDC and DAI, run the `addLiquidity.js` script:

npx hardhat run scripts/addLiquidity.js

This script performs the following steps:
- Impersonates a specific account for liquidity addition.
- Approves the Uniswap router to spend both USDC and DAI on behalf of the account.
- Adds liquidity to the USDC-DAI pool using Uniswap's `addLiquidity` function.
- Prints account balances before and after adding liquidity.

## Screenshots

### interaction with adding liquidity
<img src="https://github.com/pope-h/Uniswap_Fork_Test/blob/da13801d7437e77e974ad420fe0a8d2ce721a4e6/InteractionImages/addLiquidity.png">

### interaction with tokensForTokensSupportingFeeOnTransferTokens
<img src="https://github.com/pope-h/Uniswap_Fork_Test/blob/da13801d7437e77e974ad420fe0a8d2ce721a4e6/InteractionImages/tokensForTokensSupportingFeeOnTransferTokens.png">
*/

// Configuration

/*
Ensure you have configured the following parameters in the scripts:
- Contract addresses for USDC, DAI, and WETH.
- Router address for Uniswap.
- Victim address (the account used for impersonation).
*/

// Disclaimer

/*
These scripts are provided for educational purposes only. Use them at your own risk. Ensure you understand the transactions being performed and their implications on your accounts.
*/