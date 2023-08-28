---
title: "VaultDB: A Deployment of Secure Multiparty Computation for Clinical Research"
date: 2023-08-26 02:30:00 -0800
categories: [Healthcare, Private Analytics]
toc: true
image:
    path: notion://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F4fb68682-34f4-4a82-b990-0a06e1eec183%2FUntitled.png?table=block&id=ad35f427-e6df-4225-9963-d9d7e03d2b62&spaceId=85d84701-7672-4213-b7b6-d2de90f117b7&width=2000&userId=4437e3b9-e2de-4cb0-890e-b0aa85895308&cache=v2
author: jennie
---

VaultDB is a federated database for running SQL queries over secure multiparty computation.  In this study, we deployed VaultDB within three healthcare institutions in the Chicago metropolitan area to compute a public health study identifying underserved communities of hypertension sufferers stratified by their gender, ethnicity, and race.  It also calculates the percentage of patients with fractured care (served by greater than one healthcare site).  This three-year study computes over 1M real patient rows and it is fully HIPAA compliant.  The study workflow deduplicates patients, aggregates the data, and automatically redacts its query answers to preserve data anonymity.

### Links

Rogers, Jennie, Elizabeth Adetoro, Johes Bater, Talia Canter, Dong Fu, Andrew Hamilton, Amro Hassan et al. "VaultDB: A Real-World Pilot of Secure Multi-Party Computation within a Clinical Research Network." arXiv preprint arXiv:2203.00146 (2022). [pdf](https://arxiv.org/pdf/2203.00146.pdf)
