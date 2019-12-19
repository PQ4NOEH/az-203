+++
title = " Events driven azure solutions"
description = "Event driven azure solutions"
weight = 4
pre ="<i class='fas fa-envelope-open-text'></i> "
+++ 

## Introduction
Azure offers three diferent solutions for event driven apps:
1. Azure event Grid
2. Azure Notifications Hub
3. Azure Event Hub


## event Structure

```
[
  {
    "topic": string,
    "subject": string,
    "id": string,
    "eventType": string,
    "eventTime": string,
    "data":{
      object-unique-to-each-publisher
    },
    "dataVersion": string,
    "metadataVersion": string
  }
]
```

+ Topic. The full resource path to the event source. Event Grid provides this value.
+ Subject. Publisher-defined path to the event subject.
+ eventType. One of the registered event types for this event source. This is a value you can create filters against, e.g. CustomerCreated, BlobDeleted, HttpRequestReceived, etc.

## Azure event grid
[ref](https://docs.microsoft.com/en-us/azure/event-grid/)
Azure is a simple to use message broadcast system

1. Dinamically scalable
2. Low cost
3. Serverless
4. At least once delivery
5. Push based (keep an eye with high demands it would scale the listeners on demand)


## Azure Event Hub
[ref](https://docs.microsoft.com/en-us/azure/event-hubs/)

Think of it as the enterprise broadcast system it is like Azure event Grid but for the enterprise.
It allows :

+ Massive data ingestion: It is able to receive and process over millions of events per second 
+ Allow complex authorization excenarios
+ Low latency
+ At least once delivery
+ Azure Event Hubs cares about two things: ordering and throughput

## choose between MOS solution

