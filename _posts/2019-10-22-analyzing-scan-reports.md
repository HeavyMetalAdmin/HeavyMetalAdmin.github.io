---
title: Analyzing Scan Reports
date: 2019-10-22 11:00:00
categories: [Vulnerability Management, Reports]
tags: [cvss, vulnerability_management, cysa+, terminology]
seo:
  date_modified: 2020-02-05 11:52:10 -0500
---

## Scan Reports

* Description
* Name of the vulnerability
* See Also
* Output
  * Verbatim out of the probed system
* Port
* Hosts
  * List all hosts with this Vulnerability
* CVSS (Command Vulnerability Scoring System)

## CVSS

* Access Vector
  * How to access the Vulnerability
  * Values
    * Local (L)
      * Physical or logical access
    * Adjacent Network (A)
      * Local network access
    * Network (N)
      * Remote exploit
* Access Complexity
  * Difficulty of Exploit
  * Values
    * High (H)
      * Specialized conditions
    * Medium (M)
      * Somewhat specialized conditions
    * Low (L)
      * No special conditions
* Authentication
  * Levels of authentication need for exploit
  * Values
    * Multiple (M)
      * 2 or more
    * Single (S)
      * 1
    * None (N)
* Confidentiality
  * Disclosed info if exploited
  * Values
    * None (N)
    * Partial (P)
      * Some information attacker does not control what info
    * Complete (C)
      * All info on system
* Integrity
  * Type of info alteration
  * Values
    * None (N)
    * Partial (P)
      * Some info can be altered, attacker cannot choose what info
    * Complete (C)
      * Total compromise
* Availability
  * Service disruption
  * Values
    * None (N)
    * Partial (P)
      * Degraded performance
    * Complete (C)
      * System Down

![](/uploads/cvss.png){: width="759" height="580"}

## Base Score of CVSS

![](/uploads/basescore.png){: width="887" height="438"}

### Summary:

Vulnerability MGMT programs can give good & bad information. Vulnerability scanners can rank the vulnerabilities by the CVSS when scanned. Analysts should verify results manually if they are unsure about the report legitimacy. Analyst should be familiar with the different types of attacks.