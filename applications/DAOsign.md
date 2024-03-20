# DAOsign

- **Team Name:** DAOsign
- **Payment Address:** 13s3c37rwrZfa8WQcZPdqE1zi1hGAguf2TWfWMr8f5aLBrg

## Project Overview :page_facing_up:
### Overview


DAOsign is a WEB3 Backoffice built with Decentralized Smart Signature protocol

DAOsign offers a decentralized and customizable platform where collaboration, authorization, and workflow management are facilitated through cryptographic proofs stored on a blockchain

The Decentralized Smart Signature protocol serves as the cornerstone technology of DAOsign, encompassing a comprehensive system of cryptographic proofs, including identity, authority, signature, and agreement.

With Smart Signature, users gain access to a secure and customizable workflow management system. It also allows for control over team authorities and the ability to verify the signet’s identity.

On October 2023, our team received a grant from a Web3Foundation and we're working on our platform to be deployed on the Polkadot. Currently, DAOsign is supporting Polkadot Testnet. Polkadot Ink! implementation of DAOsign's smart contracts for creating, storing, and validating Agreement Proofs: https://github.com/DAOsign/polkadot-smart-contracts

DAOsign use cases:
- Single Document Signing
- Commodities Trading
- RWA Tokenization Backoffice
- Staking Operations and Assets Management
- Grant Programs Management
- Human Authorship Verification
- DAO Treasury Management

### Ink! Ecosystem Impact

DAOsign fit the Infrastructure category. DAOsign can fit into this ecosystem by providing a platform for all web3 companies to manage their decision-making processes/to streamline and simplify all kinds of workflows in a decentralized manner. Our target audience is not only DAOs, but also all the companies, who have a need to deal with the agreement/policies management. 

### Project Details

DAOsign consists of two components: Smart Signature and Workflow Orchestration. 

![image](https://github.com/TetianaRiabova/Ecosystem-Grants/assets/122782612/44b4a2a0-6054-46e9-9efb-5e515f4db23b)
![image](https://github.com/TetianaRiabova/Ecosystem-Grants/assets/122782612/78410abe-b4a0-4e86-b300-ba225194a9be)

Our Smart signature protocol is open-sourced and consists of three components: 
1. Agreement
2. Identity
3. Authority

![image](https://github.com/TetianaRiabova/Ecosystem-Grants/assets/122782612/71ba632d-012c-4081-ac6f-12e8eb92e0ab)



A project goal is to store Agreements Proofs on Polkadot chain using ink! smart contracts.

**Technical design**

Proofs are implemented in the EIP-712 standard and adjusted to ink! ecosystem. Proofs digned using user’s EVM private key. We are supporting this standard in Ink! smart contract to be able to verify the signature in ink! smart contract. Also, we are implementing an adjusted EIP-2771 standard to allow Agreement Signers gas-free delegation to publish proof on-chain. EIP-712 standard will be used for proofs, adaptation means that user data is converted to a binary bit; we use its hash (serialization vs deserialization) And EIP-2771 standard - to securely send the proof and receive it. So that EVM standards will be adapted to ink! ecosystem requirements.

**Off-chain Relayer**

Relayer is an off-chain component that accepts transaction (with EIP-712 signature from Metamask) from user, 
signs it and sends to the network. This app will be developed using following technology stack:

* Typescript/NodeJS
* express.js
* polkadot.js

**Architectural diagram**
![image](https://github.com/TetianaRiabova/Ecosystem-Grants/assets/122782612/468ece31-70a3-4647-ad53-ac88049de2a9)

**Definitions**:
* **Creator**: Author of agreement, define agreement content, signers
* **Signer**: Participant (Signer) of the agreement. Signs and sends transactions to a Relay
* **Relayer**: Receives signed requests off-chain from Signers and pays gas to turn it into a valid transaction that goes through a Trusted Forwarder
* **Trusted Forwarder**: A contract trusted by the Recipient to correctly verify signatures before forwarding the request from Signers
* **AgreementProof**: A contract that holds metadata and proofs for agreement.er


Agreement Proof entity represent 3 proofs:
* Proof of signature
* Proof of authority
* Proof of agreement

## Team :busts_in_silhouette:

### Team members

- Eugene Fine (CEO & Founder)
- Ramil Amerzyanov (CTO)
- Mikhail Kondratenko (Technical Lead)
- Oleksandra Burmenska (Head of Partnerships)

### Contact

- **Contact Name:** Eugene Fine
- **Contact Email:** eugene@daosign.org
- **Website:** https://daosign.org/

### Legal Structure

- **Registered Address:** 2468 Brian Dr. Northbrook, IL 60062
- **Registered Legal Entity:** DAOsign, LLC

### Team's experience

**Eugene Fine (CEO & Founder)** - Over 20 years of building, scaling, and managing technology organizations. Recent experience includes a CTO role at Explorer Surgical Corp., which was recently acquired by GHX, and VP of Engineering at GHX. Eugene is a founder at consideritdone.tech, a Blockchain/WEB3 development studio.
GitHub: https://github.com/ConsiderItDone
LinkedIn link: https://www.linkedin.com/in/eugenefine/

**Ramil Amerzyanov (CTO)** - 15+ years building complex technical architecture and software solutions., focusing on Blockchain/WEB3 technologies over the past 7 years. Recent projects include the Fractional CTO role at Landslide Network and CTO role at consideritdone.tech.
GitHub: https://github.com/ramilexe
LinkedIn link: https://www.linkedin.com/in/ramil-amerzyanov/


**Mikhail Kondratenko (Technical Lead)** - 6+ years developing Blockchain/WEB3 technical architecture and software solutions. Recent projects include Lead Technical Architect roles at Akiva Capital Holdings and Avalaunch.
GitHub: https://github.com/Brioline
LinkedIn: https://www.linkedin.com/in/mykhail-kondratenko-29209a205/

**Oleksandra Burmenska (Head of Partnerships)** - Over 10 years of experience in Business Development and Management roles in Technology organizations, focusing on Blockchain/WEB3 technologies over the past 5 years. Recent projects include contributions to NEAR, Axelar, GnosisSafe, and Avalanche ecosystems.
GitHub: github.com/burmenska
LinkedIn link: https://www.linkedin.com/in/oleksandra-burmenska/

### Team Code Repos

- https://github.com/DAOsign
- https://github.com/ConsiderItDone

Please also provide the GitHub accounts of all team members. If they contain no activity, references to projects hosted elsewhere or live are also fine.

- [Eugene Fine](https://github.com/ConsiderItDone)
- [Ramil Amerzyanov](https://github.com/ramilexe)
- [Mikhail Kondratenko](https://github.com/Brioline)
- [Oleksandra Burmenska](http://github.com/burmenska)

### Team LinkedIn Profiles (if available)

- [Eugene Fine](https://www.linkedin.com/in/eugenefine/)
- [Ramil Amerzyanov](https://www.linkedin.com/in/ramil-amerzyanov/)
- [Mikhail Kondratenko](https://www.linkedin.com/in/mykhail-kondratenko-29209a205/)
- [Oleksandra Burmenska](https://www.linkedin.com/in/oleksandra-burmenska/)


## Development Status :open_book:

Currently, DAOsign is on the Testnet: https://testnet.daosign.org/connect. We already support Polkadot, Sui, and Ethereum testnet blockchains. 

## Development Roadmap :nut_and_bolt:


### Overview

- **Total Estimated Duration:** 2 months
- **Full-Time Equivalent (FTE):**  2 FTE
- **Total Costs:** 24,050 USD


### Milestone 1 - DAOsign Application integration

* **Estimated Duration:** 2-3 weeks
* **FTE:**  2
* **Costs:** 12,025 USD


| Number | Deliverable                     | Specification                                                                                                                                                                                       |
|-------:|---------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|    0a. | License                         | Apache 2.0                                                                                                                                                                                          |
|    0b. | Documentation                   | We will provide both inline documentation of the code and a basic tutorial that explains how a user can                                                                                             |
|    0c. | Testing Guide                   | Core functions will be fully covered by unit tests to ensure functionality and robustness.                                                                                                          |
|    0d. | Docker                          | Dockerfile(s) provided in Milestone 1 will be used to test all the functionality delivered with this milestone.                                                                                     |
|     1. | DAOsign Ink! JS SDK             | We will publish a npm/yarn package with the logic how to interact with Smart Contract from JS                                                                                                       |
|     2. | DAOsign Application Integration | Integrate DAOsign application using SDK. DAOsign application (which is not part of this grant) will be open sourced as well. DAOsign is written using ReactJS on frontend and Typescript on backend |


### Milestone 2 - Relayer Development

* **Estimated Duration:** 2-3 weeks
* **FTE:**  2
* **Costs:** 12,025 USD


| Number | Deliverable   | Specification                                                                                                                                  |
|-------:|---------------|------------------------------------------------------------------------------------------------------------------------------------------------|
|    0a. | License       | Apache 2.0                                                                                                                                     |
|    0b. | Documentation | We will provide both inline documentation of the code and a basic tutorial that explains how a user can run Relayer and broadcast transactions |
|    0c. | Testing Guide | Core functions will be fully covered by unit tests to ensure functionality and robustness.                                                     |
|    0d. | Docker        | We will provide a Dockerfile(s) that can be used to test all the functionality delivered with this milestone.                                  |
|     1. | Gas Relayer   | Off-chain component for relaying transactions. Will be developed on Typescript/NodeJS using polkadot.js library                                |

## Future Plans

We are planning to improve and enhance our platform, discovering more features and use cases. Currently, we already support three chains, but we believe that DAOsign will be deployed on up to 100 chains. Also, we would be happy to connect with the Polkadot Ecosystem and provide our services for those who are interested. We will happily engage with the community to gather feedback for future enhancements. 

## Additional Information :heavy_plus_sign:

**How did you hear about the Bounty Program?** 
From a Search engine

**DAOsign Links**
- DAOsign Product Overview: http://product-overview.daosign.support
- DAOsign RWA Tokenization Backoffice: http://rwa-backoffice.daosign.support
- DAOsign Investor Deck: http://investor-deck.daosign.support
