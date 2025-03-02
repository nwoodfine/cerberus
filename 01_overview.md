---
permalink: /
layout: default
title: 1. Overview
nav_order: 1
summary: A step-by-step protocol for companies to securely store bitcoin investments without the need for a third-party custodian.
image: /assets/cerberus_title.png
---

IMPORTANT: This protocol is under development and not yet ready for use.
{: .label .label-red }

Overview
========

![The cerberus protocol](/assets/cerberus_title.png)

## Introduction

The cerberus protocol is a step-by-step protocol for **organisations** to securely store **bitcoin treasuries** without the need for a third-party custodian.

The protocol combines both *procedural* and *technical* guidance for bitcoin storage:
- **Procedural:** Guides for securely coordinating the creation of a wallet, funding the wallet, send and receive policies, personnel changes, and more.
- **Technical:** Open-source bitcoin hardware and software recommendations to securely distribute control, ensuring no single point of failure.

Cerberus is a fully open-source protocol, authored and reviewed by bitcoin industry veterans, taking inspiration from open-source guides such as the [Glacier Protocol](https://glacierprotocol.org/).

### Cerberus is intended for:
* **Organisations:** The bitcoin are owned by a collective entity rather than a single individual. Usually this will be an incorporated company, but it could also be a non-profit, family, or a nation-state.
* **Bitcoin treasuries:** Long-term bitcoin storage with a low transaction frequency (at most a handful of transactions per month).
* **Technically-unskilled users:** No software engineering or bitcoin expertise should be required. Just follow the steps.
* **Fast deployment:** Cerberus is designed to be lean and focused, so that your company can get going with bitcoin self-custody as quickly as possible.

### Cerberus minimum requirements
The details of what you'll need are detailed in [Preparation]({% link 02_preparation.md %}), but to avoid any surprises, users should ensure they will have access to the following:
* Three highly trusted team members
* Three [Trezor Ones](https://shop.trezor.io/product/trezor-one-white) (total cost less than USD 300)
* Three laptops (Windows, macOS, and Linux can be mix and matched)
* A printer
* Access to three [safe deposit box](https://en.wikipedia.org/wiki/Safe_deposit_box) providers—one per team member (e.g., banks or private vaults)
* A free afternoon to follow the [Setup]({ link 03_setup.md %}) section of the protocol

## Why cerberus?

```c
"Not your keys, not your bitcoin."
- Bitcoin proverb
```

Currently, the vast majority of bitcoin storage guidance is written for personal bitcoin holdings. But an organisation with a bitcoin treasury has _very different_ security needs compared to an individual.

Due to the lack of self-storage options, organisations are commonly resorting to trusted custodians. This poses serious risks, as organisations' bitcoin holdings are concentrated in honey pots that are highly attractive to potential attackers. A bitcoin custodian represents an easily-targeted, well-known single point of failure.

**Cerberus was produced as an easy-to-follow, quick-to-execute protocol to specifically address the unique requirements for companies self-storing bitcoin.**

Thanks to the amazing work of the bitcoin industry's open-source community and entrepreneurs, Cerberus is also inexpensive to set up, making highly-secure bitcoin storage accessible to even the smallest of companies.

## Key concepts
To follow the protocol, users may need to first familiarise with a few key terms:

| **Wallet** | A collection of addresses with associated private keys, generated from one seed phrase. |
| **Hardware wallet** | A device used to manage private keys offline. Don't confuse it with a "wallet"! |
| **Address** | What you share with third parties who are sending your company bitcoin. A new address should be used to receive each new transaction.
| **Private key** | Bitcoin transactions are controlled through private keys. Outgoing transactions must be signed with a corresponding private key. Often referred to as "key" in Cerberus for brevity. |
| **Seed phrase** | A string of words that can be used to restore a hardware wallet. Used as a backup in case of hardware wallet loss. |
| **Multisig** | A method of storing bitcoin that requires signatures from multiple private keys to make an outgoing transactions. |
| **Signatory** | An individual that manages a hardware wallet (and associated seed phrase) on behalf of the organisation. |

![Diagram of wallet structure](/assets/bitcoin_wallet_structure.png)
_A diagram showing the relationship between addresses, keys, wallets, seed phrases, and hardware wallets._

For a full list of reference terms, see the [glossary]({% link 09_glossary.md %} ).

## How it works

### Distributing control
Cerberus uses bitcoin _multisig_ to distribute control over your organisation's bitcoin holdings across three trusted team members, called _signatories_. Cerberus uses what's called a _2-of-3 multisig_, which means that there are three _private keys_, and any two of those keys are required to approve any outgoing transactions.

Each of the three signatories holds a _hardware wallet_ which manages their set of private keys. They also store a _seed phrase_ at a secure location that only they have access to, which acts as a backup in case anything goes wrong. Both the management and storage of the hardware wallet and seed are outlined in the protocol.

### Sending and receiving
To receive bitcoin a transaction, any of the three signatories can provide a bitcoin address to the sender. While this is a simple process, Cerberus provides guidelines to minimise the risk of the bitcoin being sent to the wrong place.

To send a bitcoin transaction, a designated "proposer" signatory should create a transaction and sign it, before sharing the signed transaction file with a designated "approver" signatory for final signature and broadcast. Cerberus provides a strict protocol for signatories to coordinate the proposal and approval to ensure that all outbound transactions are made according to the true intent of the organisation. It also covers how to process payments when one of the designated signatories is unavailable. 

### Issue Resolution
Finally, in the case of a hardware wallet failure, loss, or the replacement of a signatory (e.g., in the case of a staff termination), cerberus walks you through how to resolve the issue in a secure, prompt manner.

## Structure
The protocol is split into eight sections:

| 1 | **Overview** | A brief explainer on the purpose of the Cerberus Protocol. |
| 2 | **Preparation** | All the ingredients required before you begin. |
| 3 | **Setup ceremony** | A formal setup ceremony to ensure your company's bitcoin keys are generated in a secure environment. |
| 4 | **Receive a transaction** | How to safely receive incoming transactions from third parties. |
| 5 | **Send a transaction** | How to coordinate a secure outgoing transaction. |
| 6 | **Hardware wallet recovery** | How to restore a hardware wallet in the event of a hardware failure. |
| 7 | **Hardware wallet replacement** | Emergency procedures in the event of hardware wallet or seed loss, and how to replace a hardware wallet in the event of a signatory termination or death. |
| 8 | **Appendix** | All the extra background information that we ultimately decided to trim from the main protocol. Includes the kitchen sink. |
| 9 | **Glossary** | If there's a term you don't understand, look it up here! |

NOTE: When following the cerberus protocol, it's okay to read ahead, but bear in mind that the protocol is designed **so that you complete each task before moving onto the next one**. Trying to skip ahead and complete tasks to save time can lead to confusion and mistakes, compromising the security of your bitcoin storage.
{: .label .label-yellow }

## Warnings & disclaimers

### Liability
The cerberus protocol is used at your own risk, and the authors and contributors accept no responsibility for any losses incurred as part of the protocol's usage.

### Legal support
Although the cerberus is designed to minimise any potential conflicts, the protocol should still be supported by robust legal agreements between signatories and the organisation, outlining each party's obligations for the responsible management of bitcoin. These agreements are beyond both the scope of this protocol and the expertise of the authors. However, should the protocol prove to be popular, we hope that some enterprising lawyers would open-source some template documents!

### Accuracy of terminology
To ensure the protocol is quickly comprehensible for newcomers to bitcoin, we have simplified some of the key terminology and definitions. Some fastidious bitcoiners may take issue with these compromises, but we believe it's a worthwhile tradeoff to ensure that secure storage is as accessible as possible.
