# Overflow Reward Model

Overflow Reward Model provides utility for excess collateral in the pool to earn rewards in third-party protocols.&#x20;

### Definitions

**CBS DAO:** Users who supplied tokens to the collateral pool are eligible to vote accordingly to their shares in the pool

**LP Finance DAO:** Users who hold LPFi (Governance Token)are eligible to vote accordingly to their shares

**Layered DAO:** A Decentralized Autonomous Organization that is composed of layers, which allows two distinct DAOs to vote for decisions of the protocol

**CBS v2 Collateral Pool:** A seperate collateral pool where users can earn interest on supplied collaterals, opposed to CBS Collateral Pool

**Overflow Collateral:** Excess collaterals which are not required to back the CBS

![](<../.gitbook/assets/Screen Shot 2022-03-20 at 4.08.35 PM (1).png>)

**Interest-Earning Collateral:** Collaterals that are supplied to third-party protocols to earn interest

![](<../.gitbook/assets/Screen Shot 2022-03-20 at 4.09.02 PM.png>)

### Process

![](../.gitbook/assets/1\_Dxh2LXixFLX\_4hpS-uL-Vg.png)

1. CBS DAO members vote for distribution on lending protocols
2. CBS DAO members vote for Overflow Ratio
3. LP Finance DAO confirms CBS DAO Vote result
4. Interest-Earning Collateral distributed to lending protocols (ex. Solend, Apricot, Jet)

### Risks of Overflow Reward Model

#### Lending Protocol Exploit

If the selected lending protocol gets exploited, the overflow funds supplied would not be recoverable. In this case, the users who supplied to CBS v2 Collateral Pool would lose funds and might get liquidated.

There is no backup or insurance if this scenario occurs. CBS DAO members voted, therefore they are responsible for the loss. This will encourage CBS DAO to vote more cautiously on lending protocols and the overflow ratio.&#x20;

LP Finance DAO's role is also crucial to deny any proposals from CBS DAO that can lead to loss of funds.

**Lack of Backing Asset**

The backing asset in the collateral pool will never run out. If the funds are lost from the lending protocol exploit, it is the **"Overflow Fund"** meaning the required backing asset is not affected. Minted CBS are safely backed.

