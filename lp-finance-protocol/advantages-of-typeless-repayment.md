# Advantages of Typeless Repayment

Typeless repayment provides an arbitrage opportunity for users, which stabilizes the price of lpUSD and lpSOL to maintain the peg.&#x20;

Two scenarios will be introduced to demonstrate the arbitrage opportunities.

### If lpUSD price rises above 1 USD

**Assume 1 lpUSD = 1.05 USDC (5% Premium)**

Users can

1. Borrow 100 lpUSD
2. Swap 100 lpUSD to 105 USDC
3. Repay debt with 100 USDC and take 5 USDC profit

This process allows users to sell lpUSD for USDC to take profit, which will draw the price of lpUSD back to 1 USD.

### If lpUSD price falls below 1 USD

**Assume 1 lpUSD = 0.95 USDC (5% Discount)**

In this case, the arbitrage opportunity is not possible. As most users borrow lpUSD or lpSOL to swap to other tokens for leveraging position, let's assume the user swapped lpUSD to USDC right after borrowing.

1. User borrowed 100 lpUSD
2. User swapped 100 lpUSD to 100 USDC
3. &#x20;<mark style="color:red;">lpUSD price falls to $0.95</mark>
4. <mark style="color:red;">Swap 100 USDC to 105.26 lpUSD</mark>
5. <mark style="color:red;">Repay 100 lpUSD and take 5.26 lpUSD profit</mark>

The arbitrage opportunity is possible for existing debt positions. However, even if lpUSD price falls below $1, users can redeem the collateral without risk and in the event of mass repayment, lpUSD price will rise back to $1.
