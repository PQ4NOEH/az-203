+++
title = " Message driven azure solutions"
description = "Message driven azure solutions"
weight = 5
pre ="<i class='fas fa-envelope-open'></i> "
+++ 

## Pending

+ [queue storage vs service bus](https://docs.microsoft.com/en-us/azure/service-bus-messaging/service-bus-azure-and-service-bus-queues-compared-contrasted)

## Introduction

Use a message driven solution when sender and reciever are coupled. The sender expects the message to be processed in a given way.
A message has the following characteristics:

1. Point to point.
2. Itself aware.
3. The sender expect the message to be processed in a certain way. The integrity of the overall system may depend on both sender and receiver doing a specific job.

Azure offers two solutions for message driven applications:

1. Azure Service Bus.
2. Azure queue Storage Queues.

### Queues benefits

1. Message delivery guarantee
   1. At least once
   2. At most once
   3. FIFO
2. Transactional support.
3. Increments resilience
4. Decoupling between system components

### Disadvantages

1. Increments complexity


## Azure Queue storage

A service that uses Azure storage to store messages taht can be accessed using a simple REST interface. Queue can contain million of messages limited only by the capacity of the storage account that owns it.

## Azure Service Bus Queues

Is a message broker for enterprise applications that requires:

+ Multiple communication protocols: HTTP, AMPQ, etc
+ Data contracts.
+ Higher security requirements.
+ Cloud and on-premises scenarios.


## Which one should I use.

1. Service Bus topics
   1. Multiple receivers to handle each message
2. Service Bus queues
   1. Single receiver
   2. At most once delivery guarantee.
   3. FIFO
   4. You want your application to process messages as parallel long-running streams (messages are associated with a stream using the SessionId property on the message). In this model, each node in the consuming application competes for streams, as opposed to messages. When a stream is given to a consuming node, the node can examine the state of the application stream state using transactions.
   5. Transaction. Your solution requires transactional behavior and atomicity when sending or receiving multiple messages from a queue.
   6. Receive messages without polling the queue
   7. Role based access model.
   8. Different rights/permissions for senders and receivers.
   9. AMPQ 1.0 standard based protocol.
   10. Messages might be larger than 64kb but less than 1024KB (256kb standard)
   11. Queue wont be larger than 80GB
   12. Batch based publish and consumtion
   13. Duplicate detection.
   14. Expect migration from queue based solution to pub/sub one.
3.  Queue storage. Much more simpler solution
    1.  Audit trail of all messages that passes through the queue is required
    2.  Queue size larger than 80GB is expected
    3.  you want to track process for processing a message inside of the queue


## Queue storage Account

+ Name.
+ Location.
+ Performance.
  + Standard. Magnetic drives
  + Premium. Solid State Drives plus 99.9% SLA
+ Account kind. 
  + General purpose V.1. for Blob | files | tables | queues
  + General purpose V.2. for Blob | files | tables | queues
  + BlobStorage. specific for blobs
+ Replication.
  + Local Redundant Storage (LRS)
  + Zone Redundant Storage (ZRS)
  + Geo Redundant Storage (GRS)
  + Read-only Geo redundant Storage (RA-GRS)
+ Access Tier. Applies only to blobstorage Account kind storages
  + Cool 
  + Hot
+ Advanced propertiers
  + Secure transfer. 
    + Disabled (HTTP) 
    + Enabled (HTTPS)
  + Virtual networks
    + Accesible from all networks.
    + Accesible only from selected networks.
  + Blob soft delete
    + On. Allows to recover data in most cases when blobs o blobs snapshots are deleted.
    + Off.
  + Hierarchical namespace. The ADLS Gen2 herarchical namespace accelerates big data analytics workloads and enables file-level access control lists (ACLs)
    + Disabled
    + Enabled
+ Tags. Dinamic key values that allow to filter and group resources
+ security access model. For production apps Azure AD and SAS provides the best security model.
  + Azure AD
  + Shared KEY
  + Shared access signature (SAS). 

## Queue storage Shell commands

+ create. az storage create ...
+ list. 
  + az storage account list
+ get the connection string az storage account show-connection-string --name [storageName] -resource-group [storage id]