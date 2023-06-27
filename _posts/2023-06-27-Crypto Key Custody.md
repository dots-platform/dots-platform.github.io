---
title: Coinbase Cryptocurrency Key Custody
date: 2023-06-27 06:24:30 -0800
categories: [Crypto Wallet]
tags: [Coinbase]
toc: true
image:
    path: https://ctf-images-01.coinbasecdn.net/c5bd0wqjc7v0/3HNtoqqD2LJQLHjJZanDJE/fd370af7477d35448be6ce11cb1179bc/Wallet_SDK_HighRes2.png
---

Coinbase must secure signing keys since it custodies users’ digital assets. MPC is used for generating signatures on transactions without a central point of attack through a Threshold Signing Service (TSS). Each party’s longterm private keys are loaded onto Hardware Security Modules (HSMs) to prevent anyone from using the private keys if they do not have physical access to the HSM. Key generation and signature generation then occurs through the TSS protocol.

### Links

[Coinbase](https://www.coinbase.com/)

[What does Coinbase do with my digital assets?](https://help.coinbase.com/en/coinbase/other-topics/legal-policies/what-does-coinbase-do-with-my-digital-assets)

[Production Threshold Signing Service](https://www.coinbase.com/blog/production-threshold-signing-service)