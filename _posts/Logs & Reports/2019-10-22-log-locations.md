---
date: 2019-10-22 00:00:00
title: Log Locations
categories:
  - Linux
  - Logs
  - Methodology
description:
type: Document
tags: [Linux,Logs,Methodology]
---

## **Linux**

* /var/log
* Must logs are stored here, if an app doesn't use this directory change it
* Auth / kern / syslog / user

## **Cisco Log Levels**

* 0 Emergencies
* 1 Alerts
* 2 Critical
* 3 Errors
* 4 Warnings
* 5 Notifications
* 6 Information
* 7 Debugging

## **Windows Logs**

* All logs can viewed in Event Viewer
* Application Logs
  * Logs from programs or apps on system
* Security Logs
  * Logs resource rights and usage
  * File opened or deleted
* Setup Logs
  * Log setup during installation of apps
* System Logs
  * Logs of services that are running on Windows
* Forwarded Logs
  * Logs that are forwarded to this system
  * Windows version of Syslog