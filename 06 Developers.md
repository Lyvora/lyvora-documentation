# Developers

Lyvora is an open protocol designed for developers who want to help build the future of decentralized commerce — starting with real-world product transactions on-chain. The project is built with a modular, transparent, and security-focused architecture that welcomes community contributors.
## 2. Codebase
GitHub: [https://github.com/Lyvora](https://github.com/Lyvora)

The repository currently contains the initial structure of the project, including documentation, frontend development, and early drafts of contract architecture.

> Smart contracts are under development and will be published in this repository as they are built and tested.

## 3. Tech Stack

Lyvora is built using a modular stack that combines on-chain logic with off-chain infrastructure.

- **Blockchain:** SUI  
- **Smart Contracts:** Move language  
- **Frontend:** Next.js 
- **Backend Services:** Node.js (handles API integration and off-chain processes)  
- **Integrations:**  
  - **SaaS APIs** for shipping, delivery tracking, and logistics status  
  - **Oracle providers** compatible with SUI to bring off-chain data (e.g., delivery confirmation) on-chain  
- **Storage:**  
  - On-chain metadata (escrow IDs, timestamps, reputation)  
  - IPFS for storing evidence submitted during disputes
## 4. Smart Contract Modules

The Lyvora protocol will include the following smart contract modules:

### Escrow
- Locks buyer funds after purchase  
- Automatically releases funds upon delivery or after timeout  
- Supports SUI, stablecoins, and $LYV token  
- Includes fallback refund logic if shipment fails

### Dispute Resolution
- Activated when a buyer opens a complaint within the 48-hour window  
- Accepts evidence via IPFS hashes  
- Compares submissions with deterministic rules  
- In future versions, supports DAO-based arbitration

### Reputation
- Public reputation score tied to each wallet  
- Based on success rate, disputes, reviews, and response times  
- Updated after every transaction  
- Non-transferable and resistant to Sybil attacks

### Token Interaction
- Accepts payments in $LYV  
- Enables cashback, staking, and unlocks for premium features  
- Governance voting (to be activated post-launch)
## 5. How to Contribute

We're building Lyvora in public, and contributors are welcome.

To get involved:
- Follow issues and milestones on [GitHub](https://github.com/Lyvora)  
- Join the discussion on [Discord](https://discord.com/invite/wa3aMU5pmH)  
- Review the architecture in `/docs`  
- Help test smart contracts on testnet once available

A full contributors’ guide will be released in Q3 2025.
## 6. Security and Audits

Security is a top priority for Lyvora. All smart contracts will be audited by independent security firms before mainnet launch.

> Note: Smart contract development is still in progress. No audit has been conducted yet.

Planned security measures include:

- Open-source contracts for public review  
- Immutable logic after deployment  
- Replay protection and unique escrow identifiers  
- On-chain timers and automated fallback logic  
- Public bug bounty program during testnet phase  
- Multisig treasury management

---
## 7. Contact & Community

Join the development conversations:

- 💬 Discord: [https://discord.com/invite/wa3aMU5pmH](https://discord.com/invite/wa3aMU5pmH)  
- 🐙 GitHub: [https://github.com/Lyvora](https://github.com/Lyvora)  
- 📝 Medium: [https://medium.com/@Lyvora](https://medium.com/@Lyvora)

If you’re interested in building the future of commerce without borders or gatekeepers — you’re in the right place.
