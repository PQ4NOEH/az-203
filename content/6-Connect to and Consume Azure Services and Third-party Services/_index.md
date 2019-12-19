+++
date= "2016-03-08T21:07:13+01:00"
title= "6.- Connect to and Consume Azure Services and Third-party Services (20-25%)"
type= "index"
weight= 6
+++


## Introduction

This is the sixth part of the exam it is the 20 - 25 % of the final mark. It consits of the following points:

1. Logic apps
2. Search sevices
3. API Gateways
4. Event
5. Messages


## General concepts

[lesson](https://docs.microsoft.com/en-us/learn/modules/choose-a-messaging-model-in-azure-to-connect-your-services/2-choose-whether-to-use-message-queues-or-events)

**Message**


**Event**
Broadcating scenarios. sender are known as publisher and receiver as subscribers.
Events have the following characteristics:

1. Indicates something had happened.
2. Event might be listen by none or multiple subscriptors.
3. Fan out.
4. Publisher have no expectation about further action or subscribers.
5. Some events are discrete units and unrelated to other events.
6. Some events are partt of a related and ordered series.

**Message vs events**
use messages when your application must ensure that the them are processed if not use events.

