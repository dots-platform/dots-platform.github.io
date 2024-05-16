---
title: "Worldcoin Uniqueness Check"
date: 2024-05-16 15:00:00 +0100
categories: [Biometric]
toc: true
image:
    path: /assets/img/worldcoin-smpc.jpg
author: remco
---

Verified World ID users can prove that they are a unique human being without revealing who they are. To achieve this, the system makes sure the user has not signed up before during sign up by applying the Daugman iris code method, which relies on the inherent uniqueness of irises.

The verification of iris code uniqueness happens in MPC. Iris codes are encrypted as secret shares and distributed over multiple participants. Using the iris code SMPC protocol, the participants can compare the iris code of a user signing up against the encrypted shares without ever having to decrypt the secrets. Once uniqueness is verified, the new user’s iris code is encrypted to secret shares and added. Unlike the previous state of the art, where the iris codes needed to be decrypted for each comparison, stored iris codes in the new multiparty system always remain encrypted and only the comparison distance result is revealed.

### Code

[GitHub - Worldcoin Mpc Uniqueness Check](https://github.com/worldcoin/mpc-uniqueness-check)

### Presentation

{% include embed/youtube.html id='xQDXr8AZFGM' %}

### Links

* [Anouncement post](https://worldcoin.org/blog/announcements/worldcoin-foundation-unveils-new-smpc-system-deletes-old-iris-codes)
