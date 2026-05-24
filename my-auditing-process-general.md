# No matter how much auditing is done, it can always be exploited
- sam

### My general process

1. High lv. mindset to have -> be attacker and try to exploit/steal
2. General auditing process (repeat 11 steps loop) :

  * AI audit pass, get x-ray of what is done and AI findings
  * learn shallow
  * check CAVs, CVEs
  * check if user funds are at risk
  * development framework CVEs
  * development language CVEs ( rust memory issues , stack overflow, etc )
  * connectivity with other components ( off-chain connectivity, other protocol connection, external affair connections , etc )
  * check any cryptography ( EIPs, SIP,s BIPs, etc cryptography concept ) affected issues i.e CVEs related here
  * check chain's validator/consensus software CVEs
  * **EDGE CASES**; stuff which is not found by normal manual review or AI review i.e no CVEs, CAVs, etc .

    - to find these **EDGE CASES**; Use `invariant-driven`(always true rules/conditions of protocol), `stateful`(Adversarial state exploration) fuzzing; define the protocol rules that must always hold, then use **FUZZING** to generate multi-step attacker-like call sequences and check those rules after each run.
   
    - Adversarial state exploration means deliberately trying to drive your contract through weird, hostile, and edge-case sequences of states and calls to see where assumptions break
   

  * Deep Checking; learn entire flow and try to find way to steal or exploit or DOS or bad stuff for protocol

3. WHAT IS FORMAL TESTING ? CAN FORMAL TESTING BE INCLUDED IN THIS PROCESS
