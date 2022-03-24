# Democratized Liquidation

On LP Finance, liquidation is done in a democratized manner. Users can deposit lpUSD to the Auction Program. Auction program automatically liquidates collateral whenever the account's LTV hits 94%, leaving a profit. The process is as follows.

### lpUSD Borrower Liquidation

![](../.gitbook/assets/1\_q6AsXsJlfqpaCoIoZb1xWQ.png)

1. Account's LTV reaches 94%
2. Borrowed amount of lpUSD transferred to CBS Program
3. Collateral associated to target account transferred to Auction Program
4. Collateral tokens swapped to lpUSD

### lpSOL Borrower Liquidation

![](../.gitbook/assets/1\_LvTPSYziydXuDPgZUXbF1A.png)

1. Account's LTV reaches 94%
2. Swap lpUSD to lpSOL (Get minted amount of lpSOL)
3. Borrowed amount of lpSOL transferred to CBS Program
4. Collateral associated to target account transferred to Auction Program
5. Collateral tokens swapped to lpUSD

### Why swap back to lpUSD?

For every liquidation, the Auction Program swaps purchased collateral to lpUSD at the last step. This is in order to secure the profit and re-stake the lpUSD, so that it can be used at the next liquidation.&#x20;

This process allows Auction Participants to earn compounded profit from liquidation.

### Profit Rate Calculation

The profit rate on Auction Pool calculation is quite complex. First, when the Auction Pool volume is equal to the liquidated account's borrowed value, the profit rate would be

![](https://miro.medium.com/max/662/1\*NvMF8G4zOTgYGbUKtA2QWQ.png)

However, this is not likely to happen. Let's say Auction Program volume is at 10,000 lpUSD and the amount we need for liquidation is 1000 lpUSD. Only 10% of the funds are actually used for liquidation. In this case, the profit rate is not 6.38%, but (6.38\*0.1)%=0.638%.

Therefore, the profit rate is calculated as below.

![](../.gitbook/assets/1\_Y5SzTFXjmBTLJd1njV5YEw.png)

If the Auction Program volume increases relative to liquidation volume, the profit rate would increase. Therefore, profit rate is inversely dependent on Auction Program volume and proportionally dependent on liquidation volume.
