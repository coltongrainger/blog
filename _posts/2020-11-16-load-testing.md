---
title: Load Testing
author: Colton Grainger
date: 2020-11-16
revised:
---

### Load testing framework

- jmeter test plan
    - http 
    - grpc

    - abstract the configuration

- blazemeter runner
    - environments higher than qa07
    - no API reqs from gitlab ci

- jmeter runner from gradle
    - kicked off from gitlab ci (needs a private runner)
    - container image with jmeter

- gitlab ci
    - gradle build tool 
        - sends jmeter test plan to blazemeter runner
