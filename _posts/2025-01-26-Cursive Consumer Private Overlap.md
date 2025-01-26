---
title: Cursive Consumer Private Overlap
date: 2025-01-26 12:00:00 -0800
categories: [MPC] [FHE]
toc: true
image:
    path: https://i.imgur.com/wK895JJ.gif
author: vivek
---

Cursive built demos of private set intersection between two consumer's sets of personal data: contacts, event attendance, emails, personality quizzes, hiring compatibility and more.

The initial demos used a combination of MPC and FHE implemented in https://github.com/RiverRuby/2P-PSI. It uses interactive multi-party BFV to do a dot-product between two bitvectors to discover overlap. This was deployed at [ZKSummit11](https://www.cursive.team/blog/zk-summit) over contacts data collected with NFC, and the [Signature Singularity Residency](https://sigsing.vercel.app/) over event attendance data collected from your email.

The next demo used another combination of MPC and FHE implemented in https://github.com/cursive-team/pz-hiring. It uses non-interactive multi-party FHEW using the [Phantom-zone](https://github.com/gausslabs/phantom-zone) VM, which enabled more complex overlap logic. Specifically it privately checks if a candidate's salary requirements are below a recruiter's salary budget, detecting compatibility without revealing other information.

The final demo used a simple scheme involving computing a HMAC of the data label alongside a shared secret generated with ECDH. This serves as a PRF for the data. The HMACs for a pair Alice and Bob would be stored on a server, and a server would be trusted to check which HMACs overlap without colluding with either party to break the other party's privacy. This was implemented in https://github.com/cursive-team/connections.

### Mechanism

### Code

- Private set intersection over bitvetors: https://github.com/RiverRuby/2P-PSI
- Private hiring matcher: https://github.com/cursive-team/pz-hiring
- HMAC / PRF: https://github.com/cursive-team/connections

### Presentation

- Digital pheromones (a larger concept beyond just private overlap): https://app.devcon.org/schedule/LMCG3V
