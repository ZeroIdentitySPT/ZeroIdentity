# Zero Identity (0-ID)

<div align="center">
  <h3>The Invisible Bridge. Total Anonymity. Absolute Trust.</h3>
  <p>A decentralized, anonymous mediation service for physical peer-to-peer transactions.</p>
  <p>
    <a href="#how-it-works">How It Works</a> •
    <a href="#the-protocol">The Protocol</a> •
    <a href="#discord-integration">Discord</a> •
    <a href="#tos">Terms of Service</a>
  </p>
</div>

---

## 👁️ About Zero Identity

**Zero Identity** acts as a blind proxy for high-stakes or privacy-focused buy/sell transactions. We bridge the gap between a Buyer and a Seller who wish to remain completely anonymous to one another.

* **The Buyer** never learns the identity or appearance of the Seller.
* **The Seller** never learns the identity or appearance of the Buyer.
* **The Transaction** occurs physically at a neutral location designated by the Mediator.

We operate exclusively via **Discord**, utilizing ephemeral ticket systems to coordinate logistics without retaining user data.

## ⚙️ How It Works

We utilize a "Double-Blind Drop" system. The Mediator is the only entity that interacts with both parties.

## 💵 Funds Verification Protocol

To protect the Seller, the Mediator enforces a strict verification process at the time of the exchange.

**1. On-Site Authentication**
The Mediator brings counterfeit detection tools (UV lights, detector pens, or cash counting machines depending on transaction volume) to the meetup.
* **Step 1:** Cash is counted in front of the Buyer.
* **Step 2:** Bills are scanned for authenticity.

**2. Handling Discrepancies**
* **Insufficient Funds:** If the cash amount is lower than the agreed price, the Buyer has **5 minutes** to produce the difference. If they cannot, the transaction is voided.
* **Counterfeit Detection:** If fake currency is detected, the transaction is **immediately terminated**. The Buyer will be permanently banned from the Zero Identity platform.

**3. Asset Protection (The Fail-Safe)**
If the transaction fails due to payment issues:
1.   The Mediator **retains custody** of the item.
2.   The Buyer leaves empty-handed.
3.   The Mediator opens a new ticket with the Seller to arrange the return of the goods.

*Note: The item is NEVER handed to the Buyer until the full agreed amount is verified genuine and complete.*

```mermaid
sequenceDiagram
    participant B as Buyer (0-ID)
    participant M as Mediator (Zero Identity)
    participant S as Seller (0-ID)

    Note over B,S: Communication via Discord Ticket
    B->>M: Agrees to Price & Item
    S->>M: Agrees to Price & Item
    
    Note over M: Mediator Selects Neutral Location
    
    M->>S: Sends Coordinate A (Time T1)
    S->>M: Drops off Item
    M-->>S: Verifies Item & Seller Leaves
    
    M->>B: Sends Coordinate A (Time T2)
    B->>M: Drops off Cash/Payment
    M-->>B: Verifies Payment & Handoffs Item
    
    Note over B,S: Transaction Complete. Ticket Deleted.



