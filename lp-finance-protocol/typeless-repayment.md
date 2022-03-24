# Typeless Repayment

On LP Finance, there are two options for users to repay the debt.&#x20;

* lpUSD Debt (Repay in lpUSD, USDC)
* lpSOL Debt (Repay in lpSOL, SOL)

For repayment in alternative assets (USDC, SOL) the program does not calculate the value, but the number of tokens. If the user borrowed 1000 lpUSD, the user has an option to repay in 1000 USDC even if the price of USDC and lpUSD are different.

![](../.gitbook/assets/1\_UKm8rU6YV4XkEQ3PTauvvw.png)

If the repayment is in lpUSD or lpSOL, the tokens are burnt. Else if the repayment is in alternative assets, the tokens are stored in the pool to back the already minted CBS.

### **Free CBS**

In the event of repayment in alternative assets, initially borrowed CBS are now defined as "Free CBS". As the alternative assets are locked in the program forever to back the borrowed CBS, it cannot be repaid anymore in the same vault. As typeless repayment volume grows, more percentage of CBS will be "Free CBS", which stabilizes the backing of the stablecoins.

