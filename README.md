## Scam Token Analysis: PROG Token (Contract Address: 0x58cb23a3291305dfb3d38fd36ce4c307f2dacbe9)

This repository contains the analysis of the PROG Token contract found on Dextool and manually analyzed through Etherscan and Quick Intel.

### Red Flag 1: Hidden Buy/Sell Taxes (Potential Scam)
Problem: 
The contract includes high initial taxes for both buys and sells, set at 15% (_initBuyTax and _initSellTax).
While it's common for tokens to have taxes for liquidity and development, such high taxes (15%) without clear transparency are often indicative of a "honeypot" scam.

- Here's a [screenshot of the issue on Etherscan](screenshots/RedFlag1.png).

Explanation:
A honeypot scam means that users may find it difficult to sell the token after buying because the sell tax might be too high, resulting in large losses for the seller.

### Red Flag 2: Ownership Not Truly Renounced (Centralized Control)
Problem: 
The contract claims to be renounce ownership, but the owner retains privileges, especially over important parameters like buy/sell taxes. There is an address _purpleforggg which seems to have special privileges.

- Here's a [screenshot of the issue on Etherscan](screenshots/RedFlag2.png).

Explanation:
A truly decentralized contract should not allow the owner or any other address to manipulate critical functions. Here, _purpleforggg may still be able to alter the token’s behavior, which is another indication of potential malicious control.


