+++
title = " Message driven azure solutions"
description = "Message driven azure solutions"
weight = 5
pre ="<i class='fas fa-envelope-open'></i> "
+++ 

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
   3. FiFO
2. Transactional support


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
   2. At most once
   3. FIFO
   4. Transactions
   5. Receive messages without polling the queue
   6. Role based access model
   7. Messages might be larger than 64kb but less than 1024KB (256kb standard)
   8. Queue wont be larger than 80GB
   9. Batch based publish and consumtion
3.  Queue storage. Much more simpler solution
    1.  Audit trail of all messages that passes through the queue is required
    2.  Queue size larger than 80GB is expected
    3.  you want to track process for processing a message inside of the queue