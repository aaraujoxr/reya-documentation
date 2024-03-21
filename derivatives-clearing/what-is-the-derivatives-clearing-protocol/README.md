# What is the Derivatives Clearing Protocol

Reya Derivatives Clearing is a **non-custodial clearing protocol for derivatives instruments.** The Derivatives Clearing Protocol is the cornerstone that allows Reya to act as a self-reinforcing liquidity network. One of its distinguishing features is that it can aggregate positions from multiple markets _and_ multiple exchanges into a single margin account. In particular, this provides both traders and LPs with unprecedented capital efficiency by offsetting:

1. **Losses from one position with profits another**, and enabling leveraging of all portfolio profits immediately
2. **Margin requirements,** by recognizing the P\&L offset that can happen between positions
3. **P\&L and margin **_**across**_** exchanges,** by aggregating all positions into a single settlement and clearing layer

Connecting exchanges can be both DeFi or CeFi venues supporting the trading of any linear derivative contract (e.g., Futures, Swaps) via any on- or off-chain trading mechanism (e.g. Orderbook, AMM, Passive LP pool). By deploying its own appchain, Reya aims at providing these benefits while bringing on-chain the experience and speed of traditional centralized exchanges.

\[_Diagram with connecting exchanges_]

The basic concept in the Derivatives Clearing Protocol is that of a _collateral pool._ This is a compartment within the smart contract where margin deposits for any given market are kept and managed. Each of the user’s margin accounts is associated with one such collateral pool. Cashflow obligations are settled peer-to-pool. To make sure these are properly settled, the protocol has three main components:

1. Margin system that manages margin requirements for different settlement tokens and ensures safe levels of collateralization
2. Cross-collateralization module that manages features around collateralization with tokens other than the settlement token, as well as the auto-exchange mechanism which forces conversion to manage risk levels
3. Liquidation module that manages liquidation procedures when an account is declared liquidateable by the margin system.

<figure><img src="../../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>
