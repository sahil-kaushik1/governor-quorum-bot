 # Governance Quorum Change Agent

address - [Bot ID 0xb4e4...05907](https://explorer.forta.network/bot/0xb4e4c2584edab51f0c8ed56501d8974d1ba3bb798007a20ebf8a55d5f1410907)

## Description

This agent detects when a proposal is created to lower the quorum  and it will be affected by  [CVE-2022-31198](https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-xrc4-737v-9q75).

## Supported Chains

- Ethereum
- Optimism
- BSC     
- Polygon
- Avalanche

## Alerts

- GOVERNOR-QUORUM-UPDATE-PROPOSAL
  - Fired when a a proposal was created to lower the quorum numerator
  - Only fires when a contract has a bug affecting the previous proposal's results
  - Metadata includes the target address, new and current and value of the quorum numerator

