## Scam Token Analysis: PROG Token (Contract Address: 0x58cb23a3291305dfb3d38fd36ce4c307f2dacbe9)

### Introduction
This repository contains an analysis of the PROG Token, which was found on Dextool and manually analyzed through Etherscan and then Scanned through a crypto token contract scanner Quick Intel. Below is a detailed breakdown of potential red flags and malicious behavior within the contract.

### Red Flag 1: Hidden Buy/Sell Taxes
- The contract sets buy/sell taxes at 15%, which is unusually high and indicative of a honeypot scam.
- **[Screenshot of the Tax Issue](screenshots/RedFlag1.png)**

### Red Flag 2: Ownership Not Truly Renounced
- The contract claims to renounce ownership but allows a privileged address (`_purpleforggg`) to retain control over the token’s functionality.
- [Screenshot from Quick Intel Audit](screenshots/RedFlag2.png)

### Red Flag 3: Arbitrary Transaction Limits
- The owner can remove transaction limits at any time, allowing for potential manipulation of when users can sell their tokens.
- [Screenshot of the Limit Manipulation](screenshots/RedFlag3.png)

### Red Flag 4: ETH Funneling to a Private Address
- The swap function sends ETH to a private address during swaps, which could be used for a rug pull.
- [Screenshot of Swap Function](screenshots/RedFlag4.png)

## Quick Intel Analysis of Purple Frog (PROG)
- Honeypot Test: FAILED
- Liquidity: No liquidity lock found; 0 WETH in liquidity pool.
- Sell Tax: 100%, making it impossible for users to sell their tokens.
- Conclusion: The combination of a failed honeypot test, no liquidity lock, and high sell tax strongly suggests this token is a honeypot scam.
-[Screenshot of Quick Intel Analysis](screenshots/QuickIntel.png)

## DEXTools Analysis of Purple Frog (PROG)
Key Findings:
- Liquidity Drain: Over $41,000 removed from the liquidity pool by the owner.
- Suspicious Owner Activity: A massive sell order resulted in a drastic drop in token value.
- Price Volatility: Extreme price swings suggest a pump-and-dump scam.
- Rug Pull: Clear signs of a rug pull, with no remaining liquidity.
- Conclusion:The DEXTools analysis shows that this token is a scam, with the owner conducting a rug pull and leaving the investors trapped.
-[Screenshot of Dextools Analysis](screenshots/Dextools.png)




---

### Conclusion

Based on my analysis, this contract has multiple red flags that could indicate a malicious or scam token, including hidden taxes, lack of true decentralization, and arbitrary control over transactions. Investors should be cautious when interacting with tokens of this nature.

By conducting this analysis, I have demonstrated my ability to:
- Manually analyze smart contracts for potential vulnerabilities.
- Use blockchain tools like Etherscan and Quick Intel.
- Understand key red flags that indicate possible scams in token contracts.
