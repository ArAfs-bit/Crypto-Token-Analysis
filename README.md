## Scam Token Analysis: PROG Token (Contract Address: 0x58cb23a3291305dfb3d38fd36ce4c307f2dacbe9)

This repository contains the analysis of the PROG Token contract found on Dextool and manually analyzed through Etherscan and Quick Intel.

### Red Flag 1: Hidden Buy/Sell Taxes
- The contract has a 15% tax on both buys and sells.
- Here's a [screenshot of the issue on Etherscan](screenshots/etherscan_contract_issue.png).

### Red Flag 2: Ownership not truly renounced
- Although the contract claims to renounce ownership, `_purpleforggg` still has privileges.
- Here's a [screenshot from Quick Intel](screenshots/quickintel_redflag.png).


