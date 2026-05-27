List of Attack Vectors (for my quick reference)

currently created only for solana and ethereum

attack vectors :

1. [solana](solana)
2. [ethereum](ethereum)

## some attack vectors which interests me-

  - **FUCKING WITH ORACLE PRIZE**; oracle can be DEX contract , liquidity pool , etc vault where prize can be manipulated and protocol's fee or stuff is manipulated & or simply attacker gains alot without harming protocol. `also add reward manipulation here`
  - **UPGRADE PROXY**; attack where contract's logic can be updated by attacker ; via **no strict RBCA** or even if a protocol claims they are immutable but there are **IMPORTING EXTERNAL LIB CONTRACT WHICH HAS UPGRADING CONTRACT LOGIC STUFF**
  - **ATTACKER CAN FUCK A FLASH LOAN PROTOCOL USING ANOTHER FLASH LOAN PROTOCOL**; if a flash loan protocol is using RESERVES as Prize Oracle, taking a flash loan from same protocol or another protocol allows attacker to be `WHALE` for a transactions
