# Fuse

Fuse is an isolated interest rate market by Rari Capital. Each pool in Fuse can support different types of assets and use different interest rate curves. To lend out sOHM and/or use it as a collateral, users can enter [Olympus Pool Party Fuse pool](https://app.rari.capital/fuse/pool/18). In this pool, several assets are supported:

* sOHM
* USDC
* DAI
* ETH
* FRAX

## How to Supply Asset

1. Go to [Olympus Pool Party Fuse pool](https://app.rari.capital/fuse/pool/18).
2. On the Supply panel, select the asset you want to supply.

   ![The Supply panel](../../.gitbook/assets/supply.png)

3. Enter the amount of asset that you would like to supply. If you want to use the asset as collateral in order to borrow other assets against it, turn on the "Enable As Collateral" field.

   ![Enable as collateral](../../.gitbook/assets/collateral.png)

4. Click "Confirm". If this is your first time supplying the asset, you must approve the contract to spend your asset.
5. After the approval transaction is completed, you need to sign a second transaction to mint fsToken. fsToken represents your share in the pool and it allows you to redeem your supplied assets when you wish to withdraw them later.
6. When the mint transaction is completed, your asset will be supplied to the Fuse pool. This allows you to earn interest and also borrow other assets if you have enabled the supplied asset as collateral.

_Note: If you wish to borrow other assets against your collateral, there is a minimum borrow amount of 1 ETH in equivalent value. Because a small account may not be worth the gas fee to liquidate, this measure ensures that a liquidation is always profitable._

