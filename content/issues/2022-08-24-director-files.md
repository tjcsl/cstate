---
title: Director Files Not Loading
date: 2022-08-24T18:20:00-04:00
resolved: false
resolvedWhen: 2022-08-29T15:35:51-04:00
# You can use: down, disrupted, notice
severity: disrupted
affected:
  - Director
section: issue
---
Users are reporting that the file explorer is not loading insude the Director online editor. We currently believe that we have resolved the issue, which was linked to heavy load on Director's appservers. We have adjusted some backend parameters to make Director more performant under heavy usage.
