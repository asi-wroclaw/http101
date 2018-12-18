% HTTP 101
% Michał Zając

# HTTP

## Inception

Tim Berners-Lee @ CERN in 1989

## HTTP 0.9

Released in 1991

## HTTP 1.0

Released in 1996

## HTTP 1.1

Officially released in 1997, updated in 1999 and again in 2014

## HTTP 2.0

Officially released in 2015

# Architecture

## Client-server

![Client sending a request to the server](images/client-server.svg)\ 

# Request

## Syntax

```
<HTTP verb> <URI> <HTTP version>
[Headers]

<Body>
```

## Request example

```
POST / HTTP/1.1
Accept: application/json, */*
Accept-Encoding: gzip, deflate
Connection: keep-alive
Content-Length: 17
Content-Type: application/json
Host: www.google.pl
User-Agent: HTTPie/0.9.9

{
    "field": "test"
}
```

## Headers

## Body

# Types of requests

## GET

Used mostly for fetching resources

## HEAD

Same as GET but the response MUST NOT contain a body

## POST

Requests that the target resource processes the representation sent in the body

## PUT

Replace target resource with the one attached in the request's body

## PATCH

Partial modifications to target resource

## DELETE

Remove target resource

## Others

TRACE, OPTIONS, CONNECT

# Response

## Syntax

```
<HTTP version> <HTTP status code>
[Headers]

<Body>
```

## Response example

```
HTTP/1.1 200 OK
Alt-Svc: quic=":443"; ma=2592000; v="44,43,39,35"
Cache-Control: private, max-age=0
Content-Encoding: gzip
Content-Type: text/html; charset=ISO-8859-2
Date: Tue, 18 Dec 2018 23:07:14 GMT
Expires: -1
Server: gws
Set-Cookie: 1P_JAR=2018-12-18-23; expires=Thu, 17-Jan-2019 23:07:14 GMT; path=/; domain=.google.pl
Transfer-Encoding: chunked
X-Frame-Options: SAMEORIGIN
X-XSS-Protection: 1; mode=block
```

## 1xx status codes

Give information, for ex. 101 Switching Protocols

## 2xx status codes

This class indicates that the request was received, understood, accepted and processed successfully

ex. 200 OK

## 3xx status codes

This class indicates that the client must take additional action to complete the request

ex. 301 Moved Permamently

## 4xx status codes

This class of status code is intended for situations in which the error seems to have been caused by the client.

ex. 404 Not Found

## 5xx status codes

These status codes indicate cases in which the server is aware that it has encountered an error.

ex. 500 Internal Server Error

## 418 I'm a teapot

This code should be returned by teapots requested to brew coffee.

# Questions?

# Further reading

##

#. [Wikipedia: HTTP](https://www.wikiwand.com/en/Hypertext_Transfer_Protocol)
#. [Wikipedia: List of HTTP status codes](https://www.wikiwand.com/en/List_of_HTTP_status_codes)
#. [Wikipedia: HTTPS](https://www.wikiwand.com/en/HTTPS)
#. [IEFT: RFC7231](https://tools.ietf.org/html/rfc7231)
#. [IEFT: RFC7231](https://tools.ietf.org/html/rfc5789)

# Thanks!
