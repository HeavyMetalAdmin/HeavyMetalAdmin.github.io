---
title: WireShark
date: 2019-04-02 10:35:00
categories: [Tools]
tags: [network, wireshark]
seo:
  date_modified: 2020-01-24 11:42:35 -0500
---

Wireshark is a network sniffer & analyzer

* Layer 4 (Segment)
* Layer 3 (Packet)
* Layer 2 (Frame)
  * PDUs
* Dissectors cur into human readable format
* NIC must be in promiscuous mode for capture
  * Options
    * Can set different layers to name what it sees
    * Set limits on hours / days / size of files
  * Output
    * Leave as a temporary file, or set a name to write to a permanent file
    * Create a new file after a set time or size
* Capture Filter
  * Filters out data before, being sent into Wireshark
* Display Filter
  * Filters out data after it's been captured, faster than the capture filter
* *Best Practice*
  * *Use display filters more than capture filters*
* *Frames*
  * *Top Frame*
    * *Packets*
  * *Middle Frame:*
    * *Layer 1: 1st Bullet*
    * *Layer 2: 2nd Bullet*
    * *Layer 3: 3rd Bullet*
    * *Layer 4: 4th Bullet*
  * *Bottom Frame:*
    * *Binary or Hex*
    * *Can be highlighted by selecting above*
* *Unlimited profiles to different users*
  * *Can be exported to move to different systems*
* *Rule priority starts from the top*
* \!= not
  * Start wide and narrow down
* Traffic Types
  * Broadcast
    * Floods out every port except source port
    * DEST MAC: FF:FF:FF:FF:FF
  * Multicast
    * Flouts out to only members of that multicast group
    * DEST MAC: 0100:5eXX:XXXX
  * Unknown Unicast
    * Address that is not in the MAC table
    * Floods out every port except the source port
    * Added to the MAC table
    * If no response it keeps flooding out, until the source stops it
  * Unicast
    * Unique MAC addresses
    * Each system is it's own "domain"
  * Follow TCP Stream
    * Red = Source
    * Blue = Destination
  * Doubling of characters is because telnet is reporting it back to display on screen
* Expert Info
  * Bottom left dot
  * Can also click Analyze -&gt; Show Expert Info
  * Headings Overview
    * 1st column: Severity Levels
    * 2nd column: Summary of the message
* Service Response Time
  * Can find services that are sluggish