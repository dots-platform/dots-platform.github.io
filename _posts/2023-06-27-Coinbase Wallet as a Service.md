---
title: Coinbase Wallet as a Service
date: 2023-06-27 06:24:30 -0800
categories: [Infrastructure,  Crypto Wallet]
toc: true
image:
    path: https://coincu.com/wp-content/uploads/2023/05/image-1191.png
---

Coinbase’s Wallet as a Service (WaaS) is a set of wallet infrastructure APIs, enabling companies to create and deploy customizable wallets. Wallets built with WaaS will use MPC for generating signatures on transactions. The key is secret-shared between the end user and Coinbase. Coinbase uses public-verifiable backups in the case of an end user losing access to their device. 

The backup mechanism works by encrypting each shard of the private key under different backup keys, and providing a proof that these backups collectively encrypt the private key associated with the given public key. Then, a public key is enabled for use only after the backup recovery system has verified that it has a set of valid backups.

Coinbase also offers a "self-custody backup" solution where the user can hold both shares encrypted under strong keys.

### Code

[GitHub - coinbase/waas-sdk-react-native: Coinbase Wallet as a Service (WaaS) SDK for React Native. Enables MPC Operations for iOS and Android Devices.](https://github.com/coinbase/waas-sdk-react-native)

[GitHub - coinbase/waas-client-library-go: Coinbase Wallet as a Service (WaaS) Client Library in Go.](https://github.com/coinbase/waas-client-library-go)

### Links

[Coinbase Wallet as a Service](https://www.coinbase.com/cloud/products/waas)

[Coinbase announces Wallet as a Service. Now any company can seamlessly onboard their users to web3.](https://www.coinbase.com/blog/coinbase-announces-wallet-as-a-service-now-any-company-can-seamlessly)

[Preventing loss of crypto assets with publicly-verifiable encryption and backup](https://www.coinbase.com/blog/preventing-loss-of-crypto-assets-with-publicly-verifiable-encryption-and)

[Digital Asset Management with MPC (Whitepaper)](https://www.coinbase.com/blog/digital-asset-management-with-mpc-whitepaper)

[Cryptography and MPC in Coinbase Wallet as a Service (WaaS)](https://coinbase.bynder.com/m/687ea39fd77aa80e/original/CB-MPC-Whitepaper.pdf)