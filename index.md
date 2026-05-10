---
layout: default
title:
description: Personal website for Samuel Arogbonlo.
---

## About Me

<img class="profile-picture" src="{{ '/assets/images/profile.png' | relative_url }}" alt="Samuel Arogbonlo">

I’m a Staff Software Engineer focused on infrastructure.

Previously, I led central infrastructure reliability at [P2P.org](https://p2p.org/), a non-custodial staking provider with more than $10 billion in total value locked and institutional clients including BitGo, Ledger, Bybit, and Crypto.com. I built platform systems that made day-to-day operations easier for developers and saved the team more than $200,000 per month. I also worked on validator and restaking infrastructure, and led a Solana MEV project that reduced latency for clients by 10x.

Before P2P.org, I was an early engineer at [O(1) Labs](https://o1labs.org/), where I helped build and ship [Mina Protocol](https://minaprotocol.com/), a zero-knowledge blockchain that uses recursive zk-SNARKs to keep the chain small enough to verify efficiently. I also built infrastructure at [ChainSafe](https://chainsafe.io/), where my work spanned Filecoin and Ethereum, and at [Zeitgeist](https://zeitgeist.pm/), a Polkadot-based prediction market platform where I designed the production stack from the ground up.

My current interests are blockchain systems, on-chain finance, and AI infrastructure. I’m especially interested in systems where AI agents can take useful actions, but those actions still need safety checks, verification, auditability, and clear trust boundaries before they affect money, identity, or real-world institutions.

I actively contribute to open source infrastructure projects; some of that work is listed later. I’m currently building [Pisgah](https://pisgah.xyz/), an AI system for diagnostic workflows in Africa.

## Publications

[1] Arogbonlo, S., 2026. A Safety Layer for AI-Generated Blockchain Transactions. SSRN. A system for checking AI-generated blockchain transactions before they become irreversible, protecting smart contract systems from costly autonomous-agent mistakes. [SSRN](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6267278)

## Awards, Grants, and Fellowships

[1] Winner, ETHGlobal Cannes 2026, Dynamic track, for Pisgah. [Project](https://ethglobal.com/showcase/pisgah-0r3u4)

[2] Polkadot Fast Grant recipient, 2025, for building a decentralized freelance payments and escrow system on Polkadot. [Grant](https://github.com/Polkadot-Fast-Grants/apply/pull/6)

[3] Campus Director, Hult Prize, Landmark University, 2020.

[4] Udemy Ambassador, 2019/2020.

## Open Source

### Core blockchain

[1] Added sub-trie iterator support to go-ethereum so developers can scan only the part of Ethereum state they need, using prefix and range-limited traversal instead of reading unnecessary trie data. [Check code here](https://github.com/ethereum/go-ethereum/pull/32520)

### Cloud-native infrastructure

[2] Added internal service-specific label support to ingress-nginx so teams can route internal Kubernetes traffic without breaking the labels and configuration used for external services. [Check code here](https://github.com/kubernetes/ingress-nginx/pull/12704)

[3] Added NetworkPolicy support for Alertmanager in kube-prometheus-stack so monitoring deployments can restrict which pods are allowed to talk to Alertmanager in locked-down environments like banks and hospitals. [Check code here](https://github.com/prometheus-community/helm-charts/pull/5318)

[4] Added support for custom monitoring metrics writer roles in the Google Kubernetes Engine Terraform module, making it easier to provision GKE clusters with the right monitoring permissions through infrastructure as code. [Check code here](https://github.com/terraform-google-modules/terraform-google-kubernetes-engine/pull/2239)

### Security and secrets

[5] Improved Vault's token-renewal documentation so operators have clearer, more consistent guidance when keeping authentication tokens alive in production. [Check code here](https://github.com/hashicorp/vault/pull/29693)

### Independent projects

[6] [knetvis](https://github.com/samuelarogbonlo/knetvis). A Kubernetes NetworkPolicy visualization and testing tool for seeing what traffic rules allow before they go live.

[7] [Midnight Ops Doctor](https://github.com/samuelarogbonlo/midnight-ops-doctor). A Claude skill for diagnosing Midnight Network operational issues inside Claude Code, Codex, and Cursor.

[8] [Zero Compress](https://github.com/samuelarogbonlo/compression-layer2). A Rust compression project for reducing the cost of posting Layer 2 blockchain transaction data back to Ethereum.

[9] [Multisig Wallet](https://github.com/samuelarogbonlo/multisig-wallet). A k-of-n smart contract wallet for shared control of on-chain assets and protocol operations.

## Security and Bug Reports

[1] [Firedancer](https://docs.firedancer.io/) security report, 2026. Reported an integer-underflow bug in Firedancer's snapshot manifest parser through Immunefi. A malicious snapshot peer could make a Solana validator fail during snapshot boot, forcing it to retry or wait for another source. This was not a direct fund-theft bug, but validator availability bugs matter: in April 2026, Web3 lost more than $630M to hacks, and finding client-level issues early helps protect Solana infrastructure before failures can put users and funds at risk. [report](https://bugs.immunefi.com/dashboard/submission/75842) [PoC](https://gist.github.com/samuelarogbonlo/d128fe7f6590c0cf1088458eb17f2941)

## Teaching and Public Talks

I enjoy teaching practical infrastructure topics, especially where cloud, AI, Linux, and blockchain systems meet. Most of my talks are aimed at helping engineers reason about production systems with less confusion and more confidence.

| Year | Topic | Venue |
| --- | --- | --- |
| 2025 | Building Unbreakable Linux Systems Through Strategic Failure | MSCC Developers Conference, Mauritius. [event](https://conference.mscc.mu/speaker/8a2e498b-c50c-4078-a906-92d49e81c792) |
| 2025 | All About AI-Powered Linux Administration | MSCC Developers Conference, Mauritius. [event](https://conference.mscc.mu/speaker/8a2e498b-c50c-4078-a906-92d49e81c792) |
| 2025 | DevOps at the Crossroads: Enabling Secure Innovation Across AI, Web3 and Beyond | AI Security Engineers Community. [video](https://youtu.be/a4cfMB4wFNU) |
| 2025 | Web3 infrastructure and engineering | Web3 Amsterdam. [profile](https://web3amsterdam.com/speaker/samuel-arogbonlo/) |
| 2022 | Exposing Log-Metrics To Prometheus With Best Practice | Conf42 SRE. [video](https://www.youtube.com/watch?v=hQXBC2F8Lig) |
| 2025 | Cloud Meets Blockchain: The Role of Cloud Platforms in Decentralized Infrastructure | Cloud Lunch and Learn. [video](https://youtu.be/Hjy3IfTtrxs) |
| 2025 | Code and Cognition: Reducing Mental Overload In Modern GitHub Workflows | Internal workshop for GitHub employees |
| 2025 | Solving Simple Problems with AI and Web3 | ETH Enugu |

## Articles and Blog

I write about platform engineering, blockchain infrastructure, security, and the parts of AI that change how engineers build and operate systems.

| Date | Article | Publication |
| --- | --- | --- |
| Mar 2025 | [How We Reduced Onboarding Time From 2 Weeks to 2 Hours: A Platform Engineering Case Study](https://platformengineering.com/features/how-we-reduced-onboarding-time-from-2-weeks-to-2-hours-a-platform-engineering-case-study/). **Selected for Platform Engineering's Best of 2025 series.** [Best of 2025](https://platformengineering.com/features/how-we-reduced-onboarding-time-from-2-weeks-to-2-hours-a-platform-engineering-case-study-2/) | Platform Engineering |
| Mar 2025 | [How Generative AI is Redefining Self-Service Capabilities in IDPs](https://platformengineering.com/features/how-generative-ai-is-redefining-self-service-capabilities-in-idps/). On using GenAI to compress developer onboarding inside internal developer platforms. | Platform Engineering |
| Feb 2025 | [Security as a Mindset: How to Embed Security Into Cloud-Native Infrastructure Design](https://platformengineering.com/features/security-as-a-mindset-how-to-embed-security-into-cloud-native-infrastructure-design/). Argues security should be a design primitive, not a late-stage audit step. | Platform Engineering |
| Apr 2026 | [Blockchains Are Fast Enough for Finance. What About Cross-Chain Settlement?](https://samuelarogbonlo451608.substack.com/p/blockchains-are-fast-enough-for-finance). A response to a16z crypto's predictability thesis, arguing cross-chain settlement, not throughput, is the next real bottleneck for on-chain finance. | Substack |
| Nov 2025 | [Why Adaptor Signatures Are Difficult to Integrate in Ethereum](https://samuelarogbonlo451608.substack.com/p/why-adaptor-signatures-are-difficult). Why elegant Bitcoin cryptography breaks on Ethereum's account model, and what that means for atomic swaps. | Substack |
| Nov 2024 | [Bare Metal vs Public Cloud For Blockchain Services](https://samuelarogbonlo.medium.com/bare-metal-vs-public-cloud-for-blockchain-services-6874a3bfe95c). Operator-grade take on infrastructure tradeoffs for production blockchain workloads. | Medium |
| Nov 2024 | [Demystifying Blockchain Infrastructure: Running Validators and Nodes](https://samuelarogbonlo.medium.com/demystifying-blockchain-infrastructure-running-validators-and-nodes-0c2035560c41). A field guide from five years of running validator infrastructure in production. | Medium |
| Feb 2024 | [Securing libp2p Keys, Keypairs, and Key Hashes In Web3](https://samuelarogbonlo.hashnode.dev/securing-libp2p-keys-keypairs-and-key-hashes-in-web3-cm5l71dsi000c09l65jvcbhbj). On key management and identity primitives in peer-to-peer networks. | Personal blog |

## Projects

* **[Pisgah](https://pisgah.xyz/).** Pisgah is an AI system for diagnostic workflows in Africa. It helps coordinate the path from a doctor's order to a lab result, prescription, and medication delivery, while keeping each step verifiable for the patient, clinic, lab, and pharmacy. The goal is to reduce missed results, reused prescriptions, and paper-based handoffs in clinical systems where trust depends on clear evidence.

* **[knetvis](https://github.com/samuelarogbonlo/knetvis).** knetvis is a CLI tool for visualizing and testing Kubernetes NetworkPolicies before they go live. It shows engineers which pods and services can actually talk to each other, so teams can catch overly broad or broken security rules before they affect production clusters.

* **[Zero Compress](https://github.com/samuelarogbonlo/compression-layer2).** Zero Compress is a Rust implementation for compressing Layer 2 blockchain transaction data before it is posted back to Ethereum. The project targets the biggest cost center for many rollups: data availability. Its benchmarked average compression is 73.6%, which would make high-volume L2 systems cheaper to operate at scale.

* **[Midnight Ops Doctor](https://github.com/samuelarogbonlo/midnight-ops-doctor).** Midnight Ops Doctor is a Claude skill for backend operations on Midnight Network. It is the first Claude skill focused on diagnosing Midnight Network operational issues, helping developers debug wallet sync problems, deployment hangs, address confusion, and verification-key mismatches inside AI coding environments like Claude Code, Codex, and Cursor.

* **[Multisig Wallet](https://github.com/samuelarogbonlo/multisig-wallet).** Multisig Wallet is a k-of-n smart contract wallet that requires multiple approved signers before sensitive actions can execute. It supports arbitrary contract calls and signer-set updates, making it a small but complete example of safer shared control for on-chain assets and protocol operations.

## Website

This website is intentionally small. It is based on the same old-school Jekyll structure as the personal website that inspired it: Markdown pages, a single column, simple navigation, and almost no JavaScript.
