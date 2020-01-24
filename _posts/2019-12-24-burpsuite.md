---
title: BurpSuite
date: 2019-12-24 00:00:00
categories: [Tools]
tags: [web_app, network]
seo:
  date_modified: 2020-01-24 11:42:35 -0500
---

## Tabs

* Target
  * Treeview of domain and paths you viewed
  * Shows scope of testing
  * Gray items show that the spider found a resource but it has not been requested yet
  * Set the scope of the test
* Proxy
  * Interceptor
    * Contains the intercept which allows editing of packets
    * Header manipulation
  * HTTP History
    * Shows the pages seen by your browser
    * Shows response and request
  * WebSockets
    * Show messages sent over websockets
* Spider
  * Find useful pages or functionality
* Scanner
  * PRO only
* Intruder
  * Can be used for automated request in bulk
  * Attack Types
    * Sniper: Generates a single set of payloads in each position you mark
    * Battering Ram: Puts each paylaod in each position all at once
    * Pitchfork: Iterates over payloads at once
    * Cluster Bomb: Payload independently&nbsp; iterates over the playloads over each request
* Repeater
  * Repeat existing request but edit them for new request
* Sequencer
  * Capture and load tokens
  * Edit tokens as well
* Decoder
  * Decode and Encode data
* Comparer
  * Compare two blocks of data