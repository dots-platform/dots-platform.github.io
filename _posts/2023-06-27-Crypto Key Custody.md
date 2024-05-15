---
title: Coinbase Cryptocurrency Key Custody
date: 2023-06-27 06:24:30 -0800
categories: [Crypto Wallet]
toc: true
image:
    path: /assets/img/coinbase-custody.png
---

Coinbase must secure signing keys since it custodies users’ digital assets. MPC is used for generating signatures on transactions without a central point of attack through a Threshold Signing Service (TSS). Each party’s longterm private keys are loaded onto Hardware Security Modules (HSMs) to prevent anyone from using the private keys if they do not have physical access to the HSM. Key generation and signature generation then occurs through the TSS protocol.

### Links

[Coinbase](https://www.coinbase.com/)

[What does Coinbase do with my digital assets?](https://help.coinbase.com/en/coinbase/other-topics/legal-policies/what-does-coinbase-do-with-my-digital-assets)

[Production Threshold Signing Service](https://www.coinbase.com/blog/production-threshold-signing-service)