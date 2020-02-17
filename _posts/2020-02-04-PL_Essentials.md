---
title: Pentester Lab (Unix Badge)
date: 2020-02-04 14:51:00
categories: [Red Team, Burpsuite]
tags: [red team]
seo:
  date_modified: 2020-02-05 11:57:23 -0500
---



# Essentials

## Authentication

- Cookies can be manipulated to change values, which can lead to vulnerabilities
- Cookies sometimes have values that are encoded
- DB lookups can be abused if misconfigured to allow, variants of a registered username to allow access to a different users (admin -> aDmin)
  - Comparison is not case sensitive 
  - Can also be used with spaces (admin -> admin_ )
- Using Burp a misconfigured page can present it's source code in the Response

