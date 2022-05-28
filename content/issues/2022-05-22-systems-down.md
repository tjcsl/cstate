---
title: Web Services Down
date: 2022-05-22T05:32:40-04:00
resolved: true
resolvedWhen: 2022-05-27T21:54:00-04:00
# You can use: down, disrupted, notice
severity: down
affected:
  - AI Grader
  - Director
  - DNS
  - JupyterHub
  - Ion
  - Matterless
  - Othello
  - Signage
  - Tin
  - Webmail
section: issue
---
Several of our web services unexpectedly went down in the morning of May 22, 2022. After several days of investigation, we have restored the services to full operation.

We are not entirely sure what triggered the shutdown, but we do know that a crucial server managed by the TJHSST Tech Team crashed at some point between Friday 5/20 and Sunday 5/22, causing problems with our DNS servers (whose internal name resolution depended on said server). When we found a workaround for that issue in the evening of Sunday 5/22, we rebooted all servers. Unfortunately, one of our VM hosts experienced unexpected networking issues, causing all VMs on that host to be unavailable until they were moved to other servers on Tuesday 5/24. In addition, this reboot applied updates to kernel versions on our Ion and Director appservers, which broke communication between nodes on the Docker swarms for both services until the kernel was rolled back on Friday 5/27.
