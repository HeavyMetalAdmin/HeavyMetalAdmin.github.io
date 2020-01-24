---
title: Web Applications
date: 2019-11-05 00:00:00
categories: [Web App]
tags: [eJPT]
---

## HTTP Protocol Basics

* HTTP is the most used application protocol on the Internet.
* During HTTP communications the server and client exchange messages.
  * The client sends the request.
  * The server sends the response
* HTTP is a TCP protocol
  * TCP connection must first be established and then HTTP can proceed
  * SYN - SYN/ACK - ACK (Get /html) - HTML response - close connection
* HTTP message format
  * Headers\\r\\n
  * \\r\\n
  * Message Body\\r\\n
  * Must use \\r and \\n to end HTTP lines
  * Every header fields has the same format:
    * Header-name: header value
* Plain test, everything is in the clear

## HTTP Request Headers

* HTTP verb, request method, states type of request
  * GET
    * used to open web resources
  * / = path which tells the server which resource the browser is asking for
  * HTTP 1.1 is the protocol version tells the server how to communicate.
  * Many HTTP methods
    * PUT
    * TRACE
    * HEAD
    * POST
* Host header fields specifies the Internet hostname and port
  * Value is obtained via the URI of the resource
* User-Agent tells the server what client software is requesting the resource
* Accept header, is what the browser sends to specify which document type is requested
* Accept-Language header is the readable language the browser request
* Accept-Encoding header restricts the content encoding, not the content itself.
* Connection header allows the sender to specify options in regard to the connection

## HTTP Response Headers

* Status-Line is the first line
  * Contains:
    * Protocol version
    * Status Code
      * 200 OK
        * Resource is found
      * 301 Moved Permanently
        * Resource has been assigned a new URI
      * 302 Found
      * Resource is temporary under a new URI
      * 402 Forbidden
        * The client doesn't have enough privileges and the server refuses the request
      * 404 Not Found
        * The server cannot find a resource with for the request
      * 500 Internal Server Error
        * Server does not support the functionality required to fulfill the request
    * Textual Meaning
* Date
  * Time the message was generated
* Cache-Control
  * Informs client about cached content
  * Saves bandwidth
* Content-Type
  * Tells the client how to interpret the body of the message
* Content-Encoding
  * Tells the client the encoding on the body
* Server
  * Optional field
  * Tells the client about the server that generated the request
* Content-Length
  * Length in bytes of the message body

## HTTPS Basics

* HTTP over SSL/TLS
* Adds encryption to HTTP via a cryptographic protocol
* Does not protect against web app flaws
* Just protects the data exchanged between the client and server

## HTTP Cookies

* HTTP is stateless, sites don't keep the state of visitors
* Cookies invented in 1994 by Netscape
* Cookie Jar stores the cookies for the browser
* Servers can set a cookie via Set-Cookie header
  * Content of the cookie
    * ID=Value;
  * Expiration date
    * expires=Thu, 21-May-2020
    * 15:25:20 GMT;
  * Path
    * path=/example/path;
      * Will only send cookies to this path
  * The domain
    * domain=.example.site;
    * When a cookie has the domain attribute set to:
      * domain=elearnsecurity.com or
      * domain=.elearnsecurity.com
      * The browser sends the cookie to all subdomains
  * Optional flags:
    * HTTP only
      * HttpOnly;
      * Prevents JS, Flash, and Java from reading the cookie via XSS
    * Secure flag
      * Secure
      * Only Sends via HTTPS

## Sessions

* Mechanism that lets sites store variables specific for a given visit, server side
* Identified by a session id
* Installed by sessions cookies
* Session Cookies
  * Contains a single parameter value pair
    * Session:
    * PHPSESSID:
    * JSESSIONID:
  * Can be installed after a browser performs a specific activity
  * Session IDs can also be transmitted via GET request

## Same Origin Policy

* Prevents JS from getting or setting properties on a resource coming from a different origin.
* &nbsp;