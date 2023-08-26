---
title: VaultDB: A Deployment of Secure Multiparty Computation within a Clinical Research Network
date: 2023-08-26 14:30:00 -0800
categories: [Healthcare, Private Analytics]
toc: true
image:
    path: http://users.eecs.northwestern.edu/~jennie/images/vaultdb-crn-arch-detail.png 
author: jennie
---


![Data Flow Diagram](http://users.eecs.northwestern.edu/~jennie/images/vaultdb-crn-arch-detail.png)

VaultDB is a federated database for running SQL queries over secure multiparty computation.  In this study, we deployed VaultDB within three healthcare institutions in the Chicago metropolitan area to compute a public health study identifying underserved communities of hypertension sufferers stratified by their gender, ethnicity, and race.  It also calculates the percentage of patients with fractured care (served by greater than one healthcare site).  This three-year study computes over 1M real patient rows and it is fully HIPAA compliant.  The study workflow deduplicates patients, aggregates the data, and automatically redacts its query answers to satisfy anonymity requirements.


### Links

[arxiv](https://arxiv.org/abs/2203.00146)