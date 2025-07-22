#  Protocol
The Lyvora protocol was designed to combine the benefits of decentralization with the practicality required for trading physical products. It addresses common issues found in traditional platforms, such as high fees, arbitrary account freezes, and excessive collection of personal data.

Through auditable smart contracts and an automatic escrow custody system, Lyvora enables secure transactions without financial intermediaries. At the same time, it transparently integrates SaaS logistics services, making real-world delivery and tracking possible.

### The protocol’s philosophy combines:

* Autonomy: users have full control over their funds and data.

* Transparency: all financial stages are publicly auditable on-chain.

* Privacy: only essential data is stored off-chain.

* Efficiency: low fees and a streamlined process.

 # Transaction Flow

 ### **Flow Steps**

1️⃣ **Login with Crypto Wallet**

Users access the platform by connecting their digital wallet.

**No mandatory KYC or traditional account registration is required.**

⬇️

2️⃣ **Product Selection**

The buyer browses listings and selects the desired product.

All product prices are shown in US dollars (USD) as a reference, providing clear and consistent information for international buyers.

 ⚠️”All product prices are shown in US dollars (USD) as a reference, providing clear and consistent information for international buyers.”

⬇️

3️⃣ **Internal Chat and Negotiation**

The buyer can message the seller before purchasing.

While the chat is stored off-chain, **key records (such as the final offer) generate IPFS hashes linked on-chain**, ensuring the integrity of negotiations.

⬇️

4️⃣ **Purchase and Payment**

The buyer clicks **“Buy”** and completes payment using **SUI, stablecoins, or the Lyvora token ($LYV)**.

Payment can be made via **QR code or connected wallet**.

⬇️

5️⃣ **Escrow Contract Lock**

Funds are automatically transferred to the **escrow smart contract**, where they remain locked until all conditions are met.

⬇️

6️⃣ **Automatic Tracking**

The system synchronizes delivery status with the logistics provider automatically.

⬇️

7️⃣ **Buyer Notification**

The buyer receives a notification that the product has been shipped.

⬇️

8️⃣ **Direct Tracking**

The buyer can monitor the delivery status **directly within the platform**, in real time.

⬇️

9️⃣ **“Delivered” Status**

When the carrier confirms delivery, the order status updates to **“Delivered.”**

⬇️

🔟 **Receipt Confirmation**

The buyer marks the order as **“Received”** on the platform.

⬇️

1️⃣1️⃣ **48-Hour Review Period**

After marking as received, a **48-hour window** begins during which the buyer can:

- Confirm the product is correct
- Open a dispute

Automatic reminder messages are displayed during this period.

⬇️

1️⃣2️⃣ **Buyer Decision**

### Buyer Decision

| Situation         | Action Taken      | Result                   |
|-------------------|-------------------|---------------------------|
| ✅ Product OK      | Confirms receipt  | 💰 Payment is released     |
| ❌ Product Issue   | Opens dispute     | ⚠️ Dispute mode activated  |


⬇️

1️⃣3️⃣ **Transaction Review**

After completion, buyer and seller leave feedback.

Reputation is recorded immutably on the blockchain.

⬇️

1️⃣4️⃣ **Cashback and Rewards**

The buyer automatically receives cashback and any applicable token rewards according to the campaign rules.

---

⚡ **Scalability and Efficiency**

The entire flow is designed to operate with **low transaction fees** and high scalability, supporting thousands of users simultaneously.

# Escrow Module

Escrow is the central security component of the protocol.

## Detailed characteristics:

- Each transaction generates a unique ID linked to the buyer’s and seller’s wallet addresses and the purchased product.

- Funds are automatically locked in the smart contract.

- Release occurs only after one of the following conditions:

- Explicit confirmation by the buyer:
Once the delivery status is “Delivered,” the buyer manually confirms receipt in the Lyvora dashboard. The system displays verification prompts:

“Are you sure the product is correct?”
“Please double-check before confirming.”
If confirmed, payment is released immediately.

- Opening a dispute:
If the buyer detects an issue, they can open a dispute within the 48-hour window. Before proceeding, the system asks them to select a reason and confirm the action.

- Expiration of the review period:
If the buyer takes no action within 48 hours, the contract automatically releases the payment to the seller.

### Accepted tokens:

- SUI

- Supported stablecoins

- $LYV (Lyvora’s native token), which offers exclusive benefits.

  # Tracking and Logistics System
  The logistics layer operates via SaaS integrations connected to Lyvora’s backend.
  ### Features:

- Automatic shipping cost calculation at checkout.

- Generation of ready-to-print shipping labels.

- Periodic status updates synchronized with the buyer’s dashboard.

- Real-time delivery tracking.

Privacy Note:
Tracking information and shipping addresses are not stored on-chain. They remain securely in the platform’s backend database. Optionally, a cryptographic hash of this data can be saved on-chain as proof of integrity.
# Dispute Resolution 
### Flow:

- The buyer opens a dispute and submits evidence.

- The seller has up to 48 hours to respond.

- The decision is made based on predefined rules or mediation.

- The outcome determines whether funds are released or refunded.

- Reputation is updated on-chain.

- The detailed return process will be defined later.

  #  Reputation System
  ### Each wallet maintains an immutable history that includes:

- Completed transactions.

- Disputes and outcomes.

- Ratings received.

-Trust indicators.

In the future, the protocol may issue reputation NFTs to attest to user credibility.
 # On-Chain Events
### Events emitted by the protocol include:

- Escrow creation.

- Payment status updates.
 
- Dispute initiation and resolution.

- Ratings recorded.

These events enable public auditability and transparency.
# Future Roadmap: Oracle Integration
Currently, delivery confirmation relies on SaaS API integrations. In the future, support for public oracles (such as Chainlink and Supra Oracles) will be considered to record delivery confirmations directly on-chain. At this time, none of these solutions offer official support for SUI, but we will monitor ecosystem developments. As an alternative, Lyvora may develop its own proprietary oracle.

# $LYV Token – Present and Future Uses
### In addition to cashback, the $LYV token has strategic purposes:

- Governance: voting on proposals.

- Staking: participating in incentive pools.

- Progressive discounts: reducing fees based on staking and token usage.
  # Security and Audits
- Smart contracts audited by independent entities.

- Contracts immutable after deployment.

- Automatic refund fallback in case of failures.

- Multi-signature wallets for treasury funds.

- Bug bounty program planned before mainnet launch.








