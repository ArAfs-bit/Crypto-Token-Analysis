## Scam Token Analysis: PROG Token (Contract Address: 0x58cb23a3291305dfb3d38fd36ce4c307f2dacbe9)

### Introduction
This repository contains an analysis of the PROG Token, which was found on Dextool and manually analyzed through Etherscan and then Scanned through a crypto token contract scanner Quick Intel. Below is a detailed breakdown of potential red flags and malicious behavior within the contract.

### Red Flag 1: Hidden Buy/Sell Taxes
- The contract sets buy/sell taxes at 15%, which is unusually high and indicative of a honeypot scam.
- **[Screenshot of the Tax Issue](screenshots/RedFlag1.png)**

### Red Flag 2: Ownership Not Truly Renounced
- The contract claims to renounce ownership but allows a privileged address (`_purpleforggg`) to retain control over the token’s functionality.
- **[Screenshot from Quick Intel Audit](screenshots/RedFlag2.png)**

### Red Flag 3: Arbitrary Transaction Limits
- The owner can remove transaction limits at any time, allowing for potential manipulation of when users can sell their tokens.
- **[Screenshot of the Limit Manipulation](screenshots/RedFlag3.png)**

### Red Flag 4: ETH Funneling to a Private Address
- The swap function sends ETH to a private address during swaps, which could be used for a rug pull.
- **[Screenshot of Swap Function](screenshots/swap_eth_issue.png)**

---

### Conclusion

Based on my analysis, this contract has multiple red flags that could indicate a malicious or scam token, including hidden taxes, lack of true decentralization, and arbitrary control over transactions. Investors should be cautious when interacting with tokens of this nature.

By conducting this analysis, I have demonstrated my ability to:
- Manually analyze smart contracts for potential vulnerabilities.
- Use blockchain tools like Etherscan and Quick Intel.
- Understand key red flags that indicate possible scams in token contracts.
