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

- blazemeter runner

- gitlab ci
    - gradle build tool 
        - sends jmeter test plan to blazemeter runner
    - asserts pass / fail against datadog metrics
    - if passes, deploys to higher environment
