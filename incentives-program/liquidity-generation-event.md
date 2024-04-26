# Liquidity Generation Event

The Liquidity Generation Event (LGE) is the time when Reya Network bootstraps liquidity before the trading starts. As liquidity is essential for trading, we aim to attract as much of it as possible.

The earliest LPs are rewarded with boosts on their XPs.

Here’s an example :

The earliest LPs depositing to the pool earn a 10X boost. That means that instead of accruing (say) 50% annualized XPs, they get 500% annualized on the capital deposited in this period.

LPs depositing to the pool later might get a 2X.

In case of multiple deposits at different boosts, final boost is counted as the capital-weighted average. For example, if you deposit 10,000 rUSD at a 10X boost and 5,000 rUSD at a 2X, then your final boost is calculated as:

$$
\frac{10×10,000\mathrm{rUSD}+2×5000\mathrm{rUSD}}{15,000\mathrm{rUSD}}=7.3×
$$

LPs keep their boost on the capital deposited during LGE up until withdrawal. When you withdraw, you lose the multiplier on the withdrawn amount (but keep it on the amount you keep deposited).

* The mechanism is simple, in order to participate in the LGE, you simply need to stake assets. **The assets available to stage are USDC from Ethereum mainnet or USDC.e from supported L2s**. Additional assets will be introduced later.
* Funds on Reya Network are non-custodial and available to withdraw at any time. A withdrawal button on the dApp is coming soon to improve UX, but in the interim you can withdraw directly from the Reya Network smart contracts should you wish to do so. If you withdraw, however, you will permanently loose the XP boost on the withdrawn capital.
* The LGE starts at midday UTC on the 22nd April and lasts until midday UTC on 6th May. Reya Perp DEX will then go live, meaning trading will start, at midday UTC on 7th May.
* EVM compatible wallets can be used to connect to the LGE page. Funds can be deposited from Ethereum Mainnet, Arbitrum One, Polygon PoS, and Optimism Mainnet.\
