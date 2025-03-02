---
layout: default
title: 9. Glossary
nav_order: 9
summary: Definitions of technical terms used throughout the cerberus protocol.
image: /assets/glossary.png
---

IMPORTANT: This protocol is under development and not yet ready for use.
{: .label .label-red }

Glossary
=======

![Glossary](/assets/glossary.png)

This chapter provides definitions of technical terms used throughout the Cerberus Protocol to ensure all participants share a common understanding of the terminology.

## A

**Address**  
A unique identifier that serves as a virtual location where cryptocurrency can be sent to and from. In Bitcoin, addresses typically start with "1", "3", or "bc1" and consist of 26-35 alphanumeric characters.

**Air-gapped**  
Referring to a computer or device that is physically isolated from unsecured networks, including the internet. Air-gapped systems are used for increased security when handling sensitive cryptographic operations.

## B

**BIP39**  
Bitcoin Improvement Proposal 39, which defines the implementation of a mnemonic code or mnemonic sentence (a group of easy to remember words) for the generation of deterministic wallets.

**Blockchain**  
A distributed, decentralized, public ledger where cryptocurrency transactions are recorded in chronological order. Each block contains a cryptographic hash of the previous block, forming a chain.

**Bitcoin (BTC)**  
The first and most widely known cryptocurrency, created in 2009 by an unknown person or group of people using the name Satoshi Nakamoto.

## C

**Cold Storage**  
A method of storing cryptocurrency offline to reduce the risk of hacking or theft. Hardware wallets are a form of cold storage.

**Confirmation**  
The process of a cryptocurrency transaction being verified by the network and added to the blockchain. Each confirmation represents another block being added on top of the block containing the transaction.

**Cryptography**  
The practice and study of techniques for secure communication in the presence of adversaries. Cryptocurrencies use cryptography to secure transactions and control the creation of new units.

## E

**Electrum**  
A lightweight Bitcoin wallet that supports hardware wallets and multisignature capabilities. The Cerberus Protocol uses Electrum as its primary software interface.

**Entropy**  
In cryptography, entropy refers to the randomness collected for use in generating cryptographic keys. Higher entropy results in more secure key generation.

**Extended Public Key (xpub)**  
A key that allows the generation of all public keys in a deterministic wallet, without access to the private keys. Used in the Cerberus Protocol to set up multisignature wallets.

## F

**Firmware**  
Software that provides control, monitoring and data manipulation of engineered products and systems. In hardware wallets, firmware is the software running on the device itself.

**Fork**  
A split in the blockchain resulting in two separate chains. Can be either a hard fork (creating a new cryptocurrency) or a soft fork (backward-compatible update).

## H

**Hardware Wallet**  
A physical device designed to securely store cryptocurrency private keys offline. The Cerberus Protocol uses Trezor One hardware wallets.

**Hash**  
A function that converts an input of arbitrary length into an encrypted output of a fixed length. Cryptocurrency mining uses hashing to verify transactions.

## K

**Key Rotation**  
The practice of changing cryptographic keys periodically to limit the amount of data encrypted under a single key and to mitigate the damage from a compromised key.

## M

**Master of Ceremony (MC)**  
In the Cerberus Protocol, the designated individual responsible for guiding the setup ceremony and ensuring all signatories follow the protocol correctly.

**Multisignature (Multisig)**  
A digital signature scheme that allows a group of users to sign a single document or transaction. The Cerberus Protocol implements a 2-of-3 multisignature arrangement.

## N

**Network Fee**  
A fee paid to miners or validators to include a transaction in the blockchain. Higher fees typically result in faster confirmation times.

## P

**PIN**  
Personal Identification Number used to secure access to a hardware wallet. In the Cerberus Protocol, each signatory creates and securely stores their own PIN.

**Private Key**  
A secret number that allows cryptocurrencies to be spent. Anyone with knowledge of a private key can control the associated cryptocurrency.

**Public Key**  
A cryptographic key that can be obtained and used by anyone to encrypt messages intended for a particular recipient. In cryptocurrency, public keys are used to derive addresses.

## R

**Recovery Seed Phrase**  
A list of words (typically 12-24) that can be used to recover access to a cryptocurrency wallet if the original device is lost or damaged. Also known as mnemonic phrase or backup phrase.

**Replace-By-Fee (RBF)**  
A protocol that allows a transaction to be replaced with a new one that pays a higher fee, before it has been confirmed in a block.

## S

**Safe Deposit Box**  
A secured container usually held within a larger safe or vault, used in the Cerberus Protocol to store seed phrases securely.

**Seed Phrase**  
See Recovery Seed Phrase.

**Signatory**  
In the Cerberus Protocol, one of three individuals authorized to participate in the multisignature arrangement.

**Setup Ceremony**  
The formal procedure detailed in the Cerberus Protocol where the multisignature wallet is established with all signatories present.

## T

**Tamper-evident**  
Packaging or seals designed to reveal if unauthorized access has occurred. The Cerberus Protocol uses tamper-evident bags to store seed phrases.

**Transaction ID (TXID)**  
A unique identifier assigned to each cryptocurrency transaction, typically represented as a hexadecimal string.

**Trezor One**  
A hardware wallet device manufactured by SatoshiLabs, used in the Cerberus Protocol as the standard hardware wallet for all signatories.

## U

**UTXO (Unspent Transaction Output)**  
An output of a blockchain transaction that has not been spent and can be used as an input in a new transaction.

## W

**Wallet**  
Software or hardware that stores private and public keys and interacts with various blockchains to enable users to send and receive digital currency.

**Wallet Address**  
See Address.

**Wallet File**  
A file containing the information necessary for Electrum to interact with a multisignature wallet. Does not contain private keys when used with hardware wallets.

## X

**xpub**  
See Extended Public Key.

***

**Note:** This glossary is intended as a reference for participants in the Cerberus Protocol and is not an exhaustive list of bitcoin terminology. Terms are defined specifically as they relate to their usage within the protocol.

***