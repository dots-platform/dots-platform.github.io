---
title: Google & Apple, Privacy-Preserving COVID-19 Exposure Notifications
date: 2023-06-27 06:24:30 -0800
categories: [Private Analytics]
toc: true
image:
    path: https://duet-cdn.vox-cdn.com/thumbor/0x0:1920x1080/1200x800/filters:focal(960x540:961x541):format(webp)/cdn.vox-cdn.com/uploads/chorus_asset/file/21831792/COVID_19_Exposure_Notification_Update_9.1.20___Hero_Screens.001.jpeg
---

The Internet Security Research Group (ISRG) and the National Institute of Health (NIH) use MPC for extracting private analytics from COVID-19 Exposure Notifications from Google and Apple devices. The objective is to allow Public Health Authorities (PHAs) to collect meaningful data from user devices (e.g. the total number of exposure notification alerts) without exposing any one client’s data.

### Mechanism

![Mechanism](https://www.abetterinternet.org/images/2021.06.04-ENPA-Service-Flow.png)

- Each user’s device data is split into two shares.
- Shares are encrypted on the user device with keys from the ISRG and NIH, respectively.
- Data shares are sent to ingestion servers operated by Google and Apple, who perform device authenticity verification and load balancing without learning anything from the shares.
- Data shares are passed to the ISRG and NIH, who combine them into a partial aggregate sum.
- The ISRG and NIH each send their partial aggregate sums to a server operated by MITRE. At this point, they are combined into a complete set of metrics that can be viewed by PHAs.

### Code

[GitHub - divviup/prio-server: A Prio server implementation.](https://github.com/divviup/prio-server)

### Links

[ISRG Prio Services for Preserving Privacy in COVID-19 EN Apps](https://www.abetterinternet.org/post/prio-services-for-covid-en/)

[Apple and Google Exposure Notification Privacy-preserving Analytics (ENPA) White Paper](https://covid19-static.cdn-apple.com/applications/covid19/current/static/contact-tracing/pdf/ENPA_White_Paper.pdf)

[Prio: Private, Robust, and Scalable Computation of Aggregate Statistics](https://people.csail.mit.edu/henrycg/files/academic/papers/nsdi17prio.pdf)