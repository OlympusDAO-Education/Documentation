# Unstake sOHM

Sometimes, the Olympus website might not be accessible due to [hosting issues](https://twitter.com/FleekHQ/status/1416505712222609411). Fear not, you can still interact with the Olympus contracts to perform certain actions such as unstaking. In this guide, we will show you how to unstake sOHM tokens via [Etherscan](https://etherscan.io/).

If you have never unstaked sOHM before, there are two steps involved:

1. Approve the staking contract to spend your sOHM tokens.
2. Unstake your sOHM tokens.

If you have unstaked sOHM before, there is only one step to perform: Unstake your sOHM tokens.

## How to Approve sOHM Spending via Etherscan

1. Go to the [Write Contract section of the sOHM token contract](https://etherscan.io/address/0x04f2694c8fcee23e8fd0dfea1d4f5bb8c352111f#writeContract).
2. Check and ensure your selected network is "Ethereum Mainnet" in your wallet. Then press **Connect to Web3** to connect your wallet if you haven't done so.
3. Once it is connected, select the first option _approve_.
4. On the _spender \(address\)_ field, we would fill in the [staking contract address](../contracts/staking.md#staking). Enter this value: **0xFd31c7d00Ca47653c6Ce64Af53c1571f9C36566a**
5. On the _amount \(uint256\)_ field, fill in the amount of sOHM you would like the staking contract to spend on your behalf, and multiply it by 1e9. Alternatively, you can use [this calculator](https://docs.google.com/spreadsheets/d/1vm48OCBnVh8uah0-3Xa7HqFwmfxgcrMIWPrOllSFIvA/edit?usp=sharing) to perform the conversion for you. If you don't want to repeat this step whenever you want to unstake, you can choose a very large value. Let's say you want to allow the contract to spend up to 1e9 sOHM on your behalf, you would enter: **1000000000000000000**
6. Click **Write**.
7. Sign the transaction on Metamask and wait for it to complete.

## How to Unstake sOHM via Etherscan

1. Go to the [Write Contract section of the staking contract](https://etherscan.io/address/0xFd31c7d00Ca47653c6Ce64Af53c1571f9C36566a#writeContract).
2. Check and ensure your selected network is "Ethereum Mainnet" in your wallet. Then press **Connect to Web3** to connect your wallet if you haven't done so.
3. Once it is connected, select the last option _unstake_.
4. On the _\_amount \(uint256\)_ field, fill in the amount you wish to unstake, and multiply it by 1e9. Alternatively, you can use [this calculator](https://docs.google.com/spreadsheets/d/1vm48OCBnVh8uah0-3Xa7HqFwmfxgcrMIWPrOllSFIvA/edit?usp=sharing) to perform the conversion for you. For example, if you want to unstake 1 sOHM, fill in the value: **1000000000**
5. On the _\_trigger \(bool\)_ field, fill in the value: **true**
6. Click **Write**.
7. Sign the transaction on Metamask and wait for it to complete.

