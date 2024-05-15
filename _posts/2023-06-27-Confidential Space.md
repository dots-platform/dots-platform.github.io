---
title: Google Confidential Space
date: 2023-06-27 06:24:30 -0800
categories: [Infrastructure]
toc: true
image:
    path:  /assets/img/google.jpg
---

Google Cloud’s Confidential Space allows Google Cloud customers to deploy MPC solutions.  Confidential Spaces can facilitate data analysis and machine learning on sensitive or regulated data among distrusting parties, an effort to ease tensions between data sharing and regulatory requirements by encouraging collaboration while maintaining data privacy. One potential application includes MPC wallets, in which the sensitive operation (signature generation using the key shards) can occur within a TEE.

![Digital Asset](https://storage.googleapis.com/gweb-cloudblog-publish/original_images/Confidential_Space_1.jpg)

### Mechanism

![Mechanism](https://storage.googleapis.com/gweb-cloudblog-publish/images/Confidential_Space_collaborators.max-1100x1100.jpg)

Confidential Space runs workloads in TEEs. Combined with Container-Optimized OS, data contributors are able to establish how their data is used and which workloads are authorized to act on it.

### Links

[Introducing Confidential Space to help unlock the value of secure data collaboration](https://cloud.google.com/blog/products/identity-security/announcing-confidential-space)

[How Confidential Space and multi-party computation can help manage digital assets more securely and efficiently](https://cloud.google.com/blog/products/identity-security/how-confidential-space-and-mpc-can-help-secure-digital-assets)

[How to secure digital assets with multi-party computation and Confidential Space](https://cloud.google.com/blog/products/identity-security/how-to-secure-digital-assets-with-multi-party-computation-and-confidential-space)

[How to Transact Digital Assets with Multi-Party Computation and Confidential Space](https://codelabs.developers.google.com/codelabs/confidential-space-mpc#0)