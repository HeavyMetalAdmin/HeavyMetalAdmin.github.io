---
title: Detection Methods
date: 2019-10-22 22:00:00
categories: [AV]
tags: [av_detection,methodology]
---

### Signature-Based Detection

* Scanning code against a signature DB, for known malignant signatures
* Signatures are normally MD5 or SHA1
  * Can be altered by changing just 1 piece of the code
* Can identify known virus quickly, but can be outdated very quickly as well
* 1 definition can be used to identify numerous other malware
  * Scans just a chunk, and ignores the fluff around the actual exe or common runtime elements

### Heuristics Detection

* Scanning service is still the same
* Still compares against a DB
* Has static set of rules that defined what is malignant behavior
* Determines the likelihood with a threat score (Weighing)
* Uses a string search in the code of the malware
* Can cause false positives
* Decompiles the code into a human readable format
  * For humans to review
  * Will highlight abnormal strings
* Can make you aware of different malware that you may be unaware of from signature based detection
* Slower than signature based
* Can whitelist and blacklist programs
* Early detection, don't have to wait for vendors to update definitions
* Can also generate false negative, was harmful but not flagged

### Behavior Detection

* Scanning server monitors actions against a DB
* Looks at the processes that are running on the machine
* Has a learning process
  * Can take some time to learn what normal behavior is
  * Malware can slip in during this time
* After learning process, switches into enforcement mode
  * This is where process get blocked
* Generates false positives
* Is reactive than proactive