---
title: PacketWhisper
date: 2019-10-27 00:00:00
categories: [Tools, PacketWhisper]
tags: [network, data_exfil]
seo:
  date_modified: 2020-02-05 11:52:10 -0500
---

### DNS Overview

* Converts hostnames to IP (& IP address to hostnames)
* Port/Protocol always open on FWs
* UDP-based: Order of delivery is not guaranteed
* IPV4 & IPV6
* High-latency & low-bandwidth
* Two DNS query types: Iterative & Recursive
* Each DNS label can contain up to 63 bytes, as long as the whole domain name &lt;= 255 bytes (max 253 bytes in practice)
* A FQDN is a domain name that is completely specified in all labels in the hierarchy of the DNS, having no parts omitted
* DNS labels are case-insenstivie

### MDNS (Multicast DNS)

* Peer to peer self organizing network
* Zero-Configuration DNS-compatible service
* UDP Port 5353
* IPV4 & 6
* Queries are multicast
* Used for small networks that don't have a local Name Server

### LLMNR (Local Link Multicast Name Resolution)

* DNS-based service for resolving hosts on same local link
* UDP Port 5355
* IPV4 & 6
* Queries are multicast

### Text-Based Steganography

* Data embedded & hidden in images / digital media
* Well-known vector
  * Google for steganography / steganalysis tools
  * Restricted to images / digital media as transfer vehicle

### Text-Based / Linguistics Stego

* Examples of hiding data in text
  * 1st letter of each line extracted to reveal message
  * Every 7th word
  * Code words in communications
  * Use of spacing, fonts, themes

### Advantages of Text-Based Stego

* Gives a lot of flexibility
* Allows for hiding in plain site
* Text is a universally transferable data format
* Tailor ciphers so cloaked data conforms to whitelisted/common traffic
  * Evade DLP, prevent alerts
  * Difficult to predict and profile the cloaked data, no signatures
  * Bypass data whitelisting controls by transforming file into allowed data
* Use cipher as a form of social engineering attack vs analyst

### Cloakify Exfilitration Toolset

* Transforms any filetype into a list of harmless-looking strings
* Lets you hide the file in plain sign, transfer the file without triggering alerts
* Transfer the cloaked file however you choose, then decloak the exfiltrated file back into it's original form
* Transmits via different ciphers that you can set or select preset/
* Receiving
  * Capture the data any way you want

### Usage

* Must be run with python2.7 command