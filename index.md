---
layout: default
title:
description: Personal website for Samuel Arogbonlo.
---

## About Me

<img class="profile-picture" src="{{ '/assets/images/profile.svg' | relative_url }}" alt="Samuel Arogbonlo">

I’m a Staff Software Engineer focused on infrastructure.

Previously, I led central infrastructure reliability at [P2P.org](https://p2p.org/), a non-custodial staking provider with more than $10 billion in total value locked and institutional clients including BitGo, Ledger, Bybit, and Crypto.com.

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

[1] [ethereum/go-ethereum #32520](https://github.com/ethereum/go-ethereum/pull/32520). Add sub-trie iterator support for prefix and range-limited trie traversal.

[2] [ethereum/go-ethereum #31600](https://github.com/ethereum/go-ethereum/pull/31600). Track block-hash to base-state-root mapping for the Verkle transition.

### Cloud-native infrastructure

[3] [kubernetes/ingress-nginx #12704](https://github.com/kubernetes/ingress-nginx/pull/12704). Add support for internal service specific labels.

[4] [prometheus-community/helm-charts #5318](https://github.com/prometheus-community/helm-charts/pull/5318). Add NetworkPolicy support for Alertmanager in kube-prometheus-stack.

[5] [grafana/loki #15293](https://github.com/grafana/loki/pull/15293). Add support for indexing log attributes in OTLPConfig.

[6] [open-telemetry/opentelemetry-collector #12816](https://github.com/open-telemetry/opentelemetry-collector/pull/12816). Fix confmap handling so original types are preserved when a slice of maps is unmarshalled.

### Security and secrets

[7] [hashicorp/vault #29701](https://github.com/hashicorp/vault/pull/29701). Make vault policy read output consistent with vault policy fmt.

[8] [hashicorp/vault #29693](https://github.com/hashicorp/vault/pull/29693). Improve token renewal documentation consistency.

## Security and Bug Reports

[1] [Firedancer](https://docs.firedancer.io/) security report, 2026. Reported an integer-underflow bug in Firedancer's snapshot manifest parser through Immunefi. A malicious snapshot peer could make a Solana validator fail during snapshot boot, forcing it to retry or wait for another source. This was not a direct fund-theft bug, but validator availability bugs matter: in April 2026, Web3 lost more than $630M to hacks, and finding client-level issues early helps protect Solana infrastructure before failures can put users and funds at risk. [report](https://bugs.immunefi.com/dashboard/submission/75842) [PoC](https://gist.github.com/samuelarogbonlo/d128fe7f6590c0cf1088458eb17f2941)

## Teaching and Public Talks

[1] Speaker, MSCC Developers Conference, Mauritius, 2025. Building Unbreakable Linux Systems Through Strategic Failure. [event](https://conference.mscc.mu/speaker/8a2e498b-c50c-4078-a906-92d49e81c792)

[2] Speaker, MSCC Developers Conference, Mauritius, 2025. All About AI-Powered Linux Administration. [event](https://conference.mscc.mu/speaker/8a2e498b-c50c-4078-a906-92d49e81c792)

[3] Speaker, AI Security Engineers Community, 2025. DevOps at the Crossroads: Enabling Secure Innovation Across AI, Web3 and Beyond. [video](https://youtu.be/a4cfMB4wFNU)

[4] Speaker, Web3 Amsterdam, Amsterdam, 2025. [profile](https://web3amsterdam.com/speaker/samuel-arogbonlo/)

[5] Speaker, Conf42 SRE, 2022. Exposing Log-Metrics To Prometheus With Best Practice. [video](https://www.youtube.com/watch?v=hQXBC2F8Lig)

[6] Speaker, Cloud Lunch and Learn. Cloud Meets Blockchain: The Role of Cloud Platforms in Decentralized Infrastructure. [video](https://youtu.be/Hjy3IfTtrxs)

[7] Internal workshop, GitHub. Code and Cognition: Reducing Mental Overload In Modern GitHub Workflows.

[8] Speaker, ETH Enugu. Solving Simple Problems with AI and Web3.

## Articles and Blog

[1] How Generative AI is Redefining Self-Service Capabilities in IDPs. Platform Engineering, March 2025. On using GenAI to compress developer onboarding inside internal developer platforms. [article](https://platformengineering.com/features/how-generative-ai-is-redefining-self-service-capabilities-in-idps/)

[2] Security as a Mindset: How to Embed Security Into Cloud-Native Infrastructure Design. Platform Engineering, February 2025. Argues security should be a design primitive, not a late-stage audit step. [article](https://platformengineering.com/features/security-as-a-mindset-how-to-embed-security-into-cloud-native-infrastructure-design/)

[3] Blockchains Are Fast Enough for Finance. What About Cross-Chain Settlement? Substack, April 2026. A response to a16z crypto's predictability thesis, arguing cross-chain settlement, not throughput, is the next real bottleneck for on-chain finance. [article](https://samuelarogbonlo451608.substack.com/p/blockchains-are-fast-enough-for-finance)

[4] Why Adaptor Signatures Are Difficult to Integrate in Ethereum. Substack, November 2025. Why elegant Bitcoin cryptography breaks on Ethereum's account model, and what that means for atomic swaps.

[5] Bare Metal vs Public Cloud For Blockchain Services. Medium, November 2024. Operator-grade take on infrastructure tradeoffs for production blockchain workloads. [article](https://samuelarogbonlo.medium.com/bare-metal-vs-public-cloud-for-blockchain-services-6874a3bfe95c)

[6] Demystifying Blockchain Infrastructure: Running Validators and Nodes. Medium, November 2024. A field guide from five years of running validator infrastructure in production. [article](https://samuelarogbonlo.medium.com/demystifying-blockchain-infrastructure-running-validators-and-nodes-0c2035560c41)

[7] Securing libp2p Keys, Keypairs, and Key Hashes In Web3. Personal blog, February 2024. On key management and identity primitives in peer-to-peer networks. [article](https://samuelarogbonlo.hashnode.dev/securing-libp2p-keys-keypairs-and-key-hashes-in-web3-cm5l71dsi000c09l65jvcbhbj)

[8] How We Reduced Onboarding Time From 2 Weeks to 2 Hours: A Platform Engineering Case Study. Platform Engineering, March 2025. Selected for Platform Engineering's Best of 2025 series. [article](https://platformengineering.com/features/how-we-reduced-onboarding-time-from-2-weeks-to-2-hours-a-platform-engineering-case-study/) [Best of 2025](https://platformengineering.com/features/how-we-reduced-onboarding-time-from-2-weeks-to-2-hours-a-platform-engineering-case-study-2/)

## Projects

* **[Pisgah](https://pisgah.xyz/).** Pisgah is an AI system for diagnostic workflows in Africa. It helps coordinate the path from a doctor's order to a lab result, prescription, and medication delivery, while keeping each step verifiable for the patient, clinic, lab, and pharmacy. The goal is to reduce missed results, reused prescriptions, and paper-based handoffs in clinical systems where trust depends on clear evidence.

* **[knetvis](https://github.com/samuelarogbonlo/knetvis).** knetvis is a CLI tool for visualizing and testing Kubernetes NetworkPolicies before they go live. It shows engineers which pods and services can actually talk to each other, so teams can catch overly broad or broken security rules before they affect production clusters.

* **[Zero Compress](https://github.com/samuelarogbonlo/compression-layer2).** Zero Compress is a Rust implementation for compressing Layer 2 blockchain transaction data before it is posted back to Ethereum. The project targets the biggest cost center for many rollups: data availability. Its benchmarked average compression is 73.6%, which would make high-volume L2 systems cheaper to operate at scale.

* **[Midnight Ops Doctor](https://github.com/samuelarogbonlo/midnight-ops-doctor).** Midnight Ops Doctor is a diagnostic playbook for backend operations on Midnight Network. It helps developers debug wallet sync issues, deployment hangs, address confusion, and verification-key mismatches inside AI coding environments like Claude Code, Codex, and Cursor.

* **[Multisig Wallet](https://github.com/samuelarogbonlo/multisig-wallet).** Multisig Wallet is a k-of-n smart contract wallet that requires multiple approved signers before sensitive actions can execute. It supports arbitrary contract calls and signer-set updates, making it a small but complete example of safer shared control for on-chain assets and protocol operations.

## Website

This website is intentionally small. It is based on the same old-school Jekyll structure as the personal website that inspired it: Markdown pages, a single column, simple navigation, and almost no JavaScript.
