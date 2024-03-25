# Money on Chain: an Algorithmic Central Bank

> This document will be part of the terms and conditions of your agreement and therefore needs to contain all the required information about the project. Don't remove any of the mandatory parts presented in bold letters or as headlines (except for the title)! Lines starting with a `>` (such as this one) should be removed. Please use markdown instead of HTML (e.g. `![](image.png)` instead of `<img>`).
>
> See the [Grants Program Process](https://github.com/w3f/Grants-Program/#pencil-process) on how to submit a proposal.

- **Team Name:** Money on Chain Team
- **Payment Address:** In the case of fiat payment, please share your bank account privately with grants@web3.foundation via your contact email (see below) and enter the date when you shared the information with us (e.g. Fiat 24.12.1971, 11:59) here. Otherwise, provide the Polkadot (for USDC & USDT) payment address. Please also specify the currency. (e.g. 0x8920... (USDC))
- **[Level](https://github.com/w3f/Grants-Program/tree/master#level_slider-levels):** 1, 2 or 3

> :exclamation: *The combination of your GitHub account submitting the application and the payment address above will be your unique identifier during the program. Please keep them safe.*

## Project Overview :page_facing_up:

Cryptos are left to the volatility of the market, while people expect money to be stable. Stablecoins are bound to fiat money, which creates regulatory and other difficulties. 

1. Create a universal solution to set up a Milton Friedman-style "central bank" where the money, while never truly stable, nonetheless keeps its value around a certain X with respect to another asset or basket of assets.
2. Motivate actors to trustlessly enter the bank as liquidity providers, expecting a profit.
3. Have this central bank run wholly automatically without any government or expert oversight.

### Overview

* A solution to generate open-source stablecoin that is fully trustless, auditable, and algorithmic.  
* The first of its kind in the Polkadot environment, chronically thirsty for good stablecoins.  
* The team has already built this solution and has operated it for four years on [https://rootstock.io/], a side chain of BTC. Going to expand to Polkadot.  

### Project Details

Build a stablecoin on the Assets Pallet backed by Bitcoin (BTC) or other currencies such as Polkadot (DOT). **Start with wrapped Bitcoin (BTC) to keep the solution similar to what already works on Rootstock.**

This is not a purely algorithmic solution but a hybrid algorithmic-asset-backed system, as earlier purely algorithmic solutions failed.

The assets backing the stablecoin are kept locked in a **pallet that replaces our smart contract**, which is both completely trustless and decentralized.
No authority has access to the wallets, and the only way to release these assets is to compensate for the temporary loss of peg if it happens.
**A reputable audit firm must audit the smart contract and must be simple - already written, must only be ported to Polkadot (and re-audited there).**

Ratio of backing is 13*1. The assets covering the stablecoin are Bitcoin (BTC) - or any other assets chosen for the new solution - and so they themselves are not stable. Room must be given for significant fluctuations of up to 80 or 90 percent downwards. That is why **over-collateralization** is a necessary element.

Build a DApp which allows an open number of users to interact with the smart contracts. There are only 4 simple functions:
* Invest in the backing assets
* get back ROI based on calculated APR/APY
* purchase the stablecoin.
* trade the stablecoin before it becomes listed on other platforms.

As collateralization increases, more stablecoins will be released into the system, keeping the 13*1 ratio. This will enable the stablecoins to hold a peg even where the backing asset (BTC, DOT, etc.) loses value rapidly and significantly, e.g. in a harsh bear market. 

### Ecosystem Fit

There is nothing like this anywhere in the environment. Stablecoins like aUSD (Accala) collapse, and this seems to be the fate of all the purely algorithmic stablecoins.

- What need (s) does your project meet?

Dependence on USDC and USDT is not a long-term option and is not what Web3 is supposed to be about. The absence of decentralized stablecoins is a great flaw in the modern Web3 system, bound to be exploited and generate the worst crash in many crypto cycles.

The proposed solution hybridizes the algorithm with backing by assets.

The project fits any ecosystem because it resolves the volatility issue, which is common for all crypto, but is offered to the Web3 environment of Polkadot because we believe this is the best next step up from Bitcoin (BTC). 

The more blockchains the project runs on, the more influence it will have, which fulfils Web3's ideology of enabling multiple concurrent solutions with small differences to run in parallel.

- Target audience: 
* traders
* holders
* people wanting to hedge against bear markets
* low risk and high risk people

- Are there any other projects similar to yours in the Substrate / Polkadot / Kusama ecosystem?
  
No. Only DEXes, but we are not a DEX. Algoritmic stablecoins fail and continue to fail. 

  - If so, how is your project different?
    
N/A  

  - If not, are there similar projects in related ecosystems?
    
Yes, on RBTC, the team's own solution, Money on Chain, which we are expanding to Polkadot and porting to Substrate.  

## Team :busts_in_silhouette:

### Team members

- Name of team leader
- Names of team members

### Contact

- **Contact Name:** Full name of the contact person in your team
- **Contact Email:** Contact email (e.g. john@duo.com)
- **Website:** Your website

### Legal Structure

- **Registered Address:** Address of your registered legal entity, if available. Please keep it in a single line. (e.g. High Street 1, London LK1 234, UK)
- **Registered Legal Entity:** Name of your registered legal entity, if available. (e.g. Duo Ltd.)

### Team's experience

Please describe the team's relevant experience. If your project involves development work, we would appreciate it if you singled out a few interesting projects or contributions made by team members in the past.

If anyone on your team has applied for a grant at the Web3 Foundation previously, please list the name of the project and legal entity here.

### Team Code Repos

- https://github.com/<your_organisation>/<project_1>
- https://github.com/<your_organisation>/<project_2>

Please also provide the GitHub accounts of all team members. If they contain no activity, references to projects hosted elsewhere or live are also fine.

- https://github.com/<team_member_1>
- https://github.com/<team_member_2>

### Team LinkedIn Profiles (if available)

- https://www.linkedin.com/<person_1>
- https://www.linkedin.com/<person_2>


## Development Status :open_book:

If you've already started implementing your project or it is part of a larger repository, please provide a link and a description of the code here. In any case, please provide some documentation on the research and other work you have conducted before applying. This could be:

- links to improvement proposals or [RFPs](https://github.com/w3f/Grants-Program/tree/master/docs/RFPs) (requests for proposal),
- academic publications relevant to the problem,
- links to your research diary, blog posts, articles, forum discussions or open GitHub issues,
- references to conversations you might have had related to this project with anyone from the Web3 Foundation,
- previous interface iterations, such as mock-ups and wireframes.

## Development Roadmap :nut_and_bolt:

This section should break the development roadmap down into milestones and deliverables. To assist you in defining it, we have created a document with examples for some grant categories [here](../docs/Support%20Docs/grant_guidelines_per_category.md). Since these will be part of the agreement, it helps to describe *the functionality we should expect in as much detail as possible*, plus how we can verify and test that functionality. Whenever milestones are delivered, we refer to this document to ensure that everything has been delivered as expected.

Below we provide an **example roadmap**. In the descriptions, it should be clear how your project is related to Substrate, Kusama or Polkadot. We *recommend* that teams structure their roadmap as 1 milestone ≈ 1 month.

> :exclamation: If any of your deliverables is based on somebody else's work, make sure you work and publish *under the terms of the license* of the respective project and that you **highlight this fact in your milestone documentation** and in the source code if applicable! **Projects that submit other people's work without proper attribution will be immediately terminated.**

### Overview

- **Total Estimated Duration:** 3 months
- **Full-Time Equivalent (FTE):**  2 FTE
- **Total Costs:** 45 000 USD.

### Milestone 1 — Porting the existing solution to Polkadot

- **Estimated duration:** 3 months
- **FTE:**  2
- **Costs:** 45 000 USD

> :exclamation: **The default deliverables 0a-0d below are mandatory for all milestones**, and deliverable 0e at least for the last one.

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| **0a.** | License | Apache 2.0 / GPLv3 / MIT / Unlicense |
| **0b.** | Documentation | We will provide both **inline documentation** of the code and a basic **tutorial** that explains how a user can (for example) spin up one of our Substrate nodes and send test transactions, which will show how the new functionality works. |
| **0c.** | Testing and Testing Guide | Core functions will be fully covered by comprehensive unit tests to ensure functionality and robustness. In the guide, we will describe how to run these tests. |
| **0d.** | Docker | We will provide a Dockerfile(s) that can be used to test all the functionality delivered with this milestone. |
| 0e. | Article | We will publish an **article**/workshop that explains [...] (what was done/achieved as part of the grant). (Content, language and medium should reflect your target audience described above.) |
| 1. | Asset: algorithmic stablecoin| We will create an Asset for our Stablecoin using the Assets pallet |
| 2. | Substrate module: Collateralization | The Substrate will enable the holding of the assets that cover the stablecoin - wrapped BTC, Polkadot (DOT) and others |
| 3. | Substrate module: Pegging | The Substrate module will algoritmically reflect the purchase to sales ratio of the Stablecoin using the data from the Assets module to enable auto pegging (sales/purchases of the Asset |
| 4. | Substrate chain | Modules 1. and 2. will interact in such a way that the collateralizing asset is used to stabilize the market for the Asset being developed |
| 5. | Front end: | We will port the front end we already use and make it Polkadot/Specific.


## Future Plans

Please include here

- we will connect the DApp to a blockchain in the Polkadot environment in such a way that every parachain can benefit
- get **thorough** audits on all our products
- we will use the promotion by our partners, amongst which is Liberland and all the channels and our community already built on Rootstock
- we will allow the collateralization by more assets, including Liberland assets
- we will port the solution to other blockchain
- we will enable the use of the stablecoin on DEXes in the Polkadot Environment

## Referral Program (optional) :moneybag:

You can find more information about the program [here](../README.md#moneybag-referral-program).

- **Referrer:** Name of the Polkadot Ambassador or GitHub account of the Web3 Foundation grantee
- **Payment Address:** Polkadot/Kusama (USDT/USDC) payment address. Please also specify the currency. (e.g. 0x8920... (USDT))

## Additional Information :heavy_plus_sign:

**How did you hear about the Grants Program?** Personal recommendation by the Liberland Team, which was awarded a grant for the Liberland Blockchain.

Here you can also add any additional information that you think is relevant to this application but isn't part of it already, such as:

- The solution is all built and running on another blockchain
- The current conversion is however total and is going to be very demanding in FTE and knowledge
