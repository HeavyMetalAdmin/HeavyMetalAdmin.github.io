---
title: Proofpoint Engineering
date: 2020-01-24 10:45:00
categories: [Tools, Proofpoint]
tags: [operations]
seo:
  date_modified: 2020-01-24 11:48:25 -0500
---
## Proofpoint

### Blocking Email
- To block a domain or IP with no logging of the message, block the message in the following way:
  - Email Protection -> Email Firewall -> Rules -> Blocked
    - Add domain and save
- To block a sender if logging of the message
  - Spam Detection -> Organizational Block List

- When blocking a domain use the Email Protection -> Spam Detection -> Org
Block List
  - This retains a copy in the quarantine folder
  - No wildcards are needed, just use contains
- When blocking a sender use Email FW -> Rules -> Blocked
  - This drops the email all together


