# QXMR Staking Smart Contract Proposal

## Introduction

The QXMR token, launched as a heartfelt tribute to Qubic’s pioneering uPoW mining of XMR in Epoch 161, embodies the revolutionary spirit driving Qubic’s remarkable success, with each day fueling anticipation for new all-time highs.

Building on this momentum, our project introduces a dynamic staking model that empowers QXMR holders to actively engage with the network, transforming enthusiasm into tangible participation.

By offering flexible staking periods—weekly, 1-month, 3-month, 6-month, or 12-month—with higher APYs for longer commitments, this initiative incentivizes sustained involvement, strengthening the Qubic ecosystem.

This staking framework not only honors QXMR’s origins but also amplifies the collective drive toward Qubic’s continued growth and innovation.

To be developed by the innovative Qearn team, Serendipity and Poly. This proposal seeks a funding allocation of $20,000 USD (10B Qu @ 0.000002) to wallet: `GBBDPCKSUDPTAFOIROJCFPRLEPXBJSTMKFONPDVBHBWTPUDVFEKRYPSBLLIA`

## Business Need

Qubic’s groundbreaking uPoW mining technology marks a significant leap forward, yet mining requirements often sideline enthusiastic community members unable to mine directly, creating a divide within our ecosystem.

The QXMR staking smart contract offers a transformative solution, empowering every QXMR holder to actively participate by staking their tokens, thus bridging this gap and fostering a unified, inclusive community. By enabling stakers to earn mining-derived rewards across flexible staking periods—weekly, monthly, or up to a year—with higher APYs for longer commitments, and an optional boost-to-burn mechanism to enhance returns, this initiative ensures all members can contribute meaningfully to Qubic’s growth.

Funding this proposal will democratize participation, align stakeholder incentives, and solidify Qubic’s success as a collective, community-driven endeavor, meeting the critical need for equitable engagement in our thriving network.

## Business Model

QXMR token holders can stake their tokens in a smart contract seamlessly integrated with Qubic’s mining operations, earning rewards in Qubic proportional to their stake size and chosen duration.

An optional burn mechanism allows stakers to sacrifice a portion of their QXMR to boost their APY, enhancing returns while increasing QXMR scarcity to benefit all holders.

My current weekly mining rewards range from 25 to 30 million Qubic, will be directed to a QXMR Staking wallet and distributed as follows:
- 60% to stakers
- 30% to fund mining operations
- 5% Qubic burned
- 5% to shareholders

This transparent, incentivized structure fosters active participation, aligns stakeholder interests, and drives the Qubic network’s sustained growth and value creation.

## Functional Features
- **Staking Interface:** A sleek, intuitive UI enabling users to stake QXMR, monitor rewards, and manage burn options effortlessly.
- **Reward Distribution:** Qubic payouts calculated based on stake size and duration, ensuring fair and transparent rewards.
- **QXMR Burning:** Optional QXMR burn feature to boost APY, promoting token scarcity and enhancing value for all holders.
- **Wallet Integration:** Seamless compatibility with Qubic’s web and mobile wallets for a smooth and secure staking experience.
- **Dashboard:** Real-time analytics displaying stake performance, QXMR earnings, and lock history for informed decision-making.
- **Deflationary:** 5% of rewards is burned, reducing overall Qubic supply.
- **Shareholder Rewards:** 5% of rewards allocated to smart contract shareholders, aligning incentives across the ecosystem.

## Components to Be Developed (High-Level)

### Frontend UI:
- Similar with Qearn UI.
- Simple Lock/Unlock Form
- Burn-to-Boost Form
- Lock History table
- Analytics page of QXMR staking
- WalletConnect
- Hosted at [https://stake.qxmr.quest/](https://stake.qxmr.quest/)

### Smart Contract:
- Staking for QXMR deposits
- Reward distribution for Qubic payouts
- Optional Burn-to-Boost logic

## Technical Architecture (High-Level)
- **Smart Contract:** C++
- **Frontend:** React + Vite + Qubic Connect

## User Journey/Examples

User:
- Visits [https://stake.qxmr.quest/](https://stake.qxmr.quest/)
- Connects Qubic wallet with WalletConnect
- Chooses amount of QXMR to stake
- Selects staking period:
  - 1 Week
  - 1 Month
  - 3 Months
  - 6 Months + 0.4% QXMR Bonus
  - 12 Months + 1% QXMR Bonus
- Selects optional Burn-to-Boost APY:
  - Bronze - Burn 5% QXMR ⇒ Boost APY +10%
  - Silver - Burn 10% QXMR ⇒ Boost APY +25%
  - Gold - Burn 20% QXMR ⇒ Boost APY +50%
  - Platinum - Burn 30% QXMR ⇒ Boost APY +80%
- Stakes QXMR

***Example UI and APY (UI mockup - not representative of Serendipity's work. UI will resemble Qearn's***

![QXMR Staking Options](staking%20qxmr.png)
![QXMR Rewards Boost](rewards%20boost.png)

## Detailed Scope and Timeline

### Timeline (6-8 weeks):
- **Week 1:** Design UI mockups and smart contract architecture
- **Week 2-4:** Prototype with staking and reward functionality
- **Week 5-6:** Smart contract integration and final testing
- **Week 7-8:** Audit, IPO, and Mainnet deployment

## Milestones and Deliverables

**Milestone 1 (1 Week):**
- Create user interface mockup without logic implementation
- Smart contract architecture docs

**Milestone 2 (3 Weeks):**
- Wallet connect
- Qubic core services integration
- Develop a functional prototype implementing staking and reward distribution features
- Smart contract first version

**Milestone 3 (2 Weeks):**
- Integration of UI with smart contract
- Final smart contract with possible updates for providing better data and interaction with UI
- Smart contract test script

**Milestone 4 (2 Weeks):**
- Audit, IPO, and Mainnet deployment

## Payment Terms

**Funding Request:** $20,000 USD
- Breakdown: 100% for devs

**Disbursement**
- 20% M1: UI mockup (without functionalities), smart contract docs
- 30% M2: Alpha version of UI and smart contract
- 20% M3: All test finished beta version
- 30% M4: Mainnet deployment

## Team Composition

- **Profitphil:** Team Lead
- **Serendıpıtч:** Lead frontend UI developer
- **Poly:** Lead smart contract developer

-Website: https://www.qxmr.quest
-X: @_qxmr_token_
