---
layout: post
title:      "Deciphering Common HTTP Status Codes"
date:       2019-02-04 03:13:14 +0000
permalink:  deciphering_common_http_status_codes
---


## What is an HTTP Status Code?

Have you ever attempted to load a webpage and encountered a three-digit number instead of whatever it was that you were trying to load? This three-digit number is known as an *HTTP Status Code*. Encountering HTTP Status Codes is inevitable. HTTP Status Codes are responses presented to a client to let the client know the status of the request that they’ve made to the server—whether good or bad. These codes allow for client-side clarity, and are extremely useful to internet users and programmers alike.

### Digit Breakdown:

* 1xx – Informational 
* 2xx – Successful
* 3xx – Redirection 
* 4xx – Client Error
* 5xx – Server Error

## 1xx Status Codes

HTTP Status Codes that begin with the number one, followed by two other digits, fall into the *informational* response category. These responses communicate with the client that the request that they made was received and is still processing—1xx Status Codes can be thought of as temporary responses. 

### Common 1xx Status Codes

* **100**: communicates that *the client’s request is OK and that the client should continue forward with their request*.
* **102**: communicates that *the server has received the client’s request, but is still processing it and is unable to give a response just yet*.

## 2xx Status Codes

HTTP Status Codes that begin with the number two, followed by two other digits, fall into the *successful* response category. These responses communicate with the client that the request that they made was successfully received, understood, and accepted. 

### Common 2xx Status Codes

* **200**: communicates that *the client’s request was successful*—a 200 status code can be thought of as getting the an *OK* from the server.
* **202**: communicates *the client’s request has been received, but has not yet been fulfilled*.

## 3xx Status Codes 

HTTP Status Codes that begin with the number three, followed by two other digits, fall into the *redirection* response category. These responses communicate with the client that the request cannot be completed until further action is taken towards completing the request.

### Common 3xx Status Codes

* **301**: communicates that *the resource the client is trying to access has permanently moved*.
* **302**: communicates that* the resource the client is trying to access has been found under a different URI*.

## 4xx Status Codes

HTTP Status Codes that begin with the number three, followed by two other digits, fall into the *client error* response category. These responses communicate with the client that there is an error on their end due to either poor syntax or that the request is unable to be fulfilled.

### Common 4xx Status Codes

* **400**: communicates a *bad request*.
* **401**: communicates to the client that *they do not have correct authentication to continue forward with their request*.
* **403**: comminutes to the client that *the server received their request, but will not move forward with authorizing it*.
* **404**: communicates that *the resource that the client is attempting to access cannot be found*.


## 5xx Status Codes

HTTP Status Codes that begin with the number three, followed by two other digits, fall into the* server error* response category. These responses communicate with the client that their request has failed due to server-induced errors—while the client’s request appears to be valid, it will result in an inability to be fulfilled.

### Common 5xx Status Codes

* **500**: communicates *an internal server error*—it communicates that the server ran into an issue that has prevented them from moving forward with the request.
* **502**: communicates that *the server has encountered a bad gateway*.
* **503**: communicates that* a service is unavailable*.
* **504**: communicates that *the server encountered a gateway timeout while trying to fulfill a client’s request*.
