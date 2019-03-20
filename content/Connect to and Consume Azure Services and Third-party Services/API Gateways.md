+++
title = " API Gateways"
description = "API Gateways"
weight = 3
pre ="<i class='fas fa-door-open'></i> "
+++ 

## Introduction

API Management (APIM) helps organizations publish APIS to external, partner, and internal developers to unlock the potential of their data and services. It provides the core competencies:
1. Business insights
2. Analytics
3. Security
4. Protection

## Common scenarios
1. Securing mobile infraestructure:
    + Gain access with API keys.
    + Prevent DOS attacks by using throttling.
    + use advance security policies like JWT token validation.
2. Enabling ISV partner ecosystem. API Facade to decouple from internal implementations that are not riple for partner consumption
3. Running an internal API program.

## The system is made up of the following components
1. The API gateway is the endpoint
    + Accepts API calls and routes them to your backends
    + Verifies APPI keys, JWT tokens, certificates, ...
    + Usage quotas and rate limits
    + Transform API in the fly without code modifications
    + Caches backend responses
    + Logs call metadata for analytics purposes.
2. The Azure portal is the administrative interface
3. The Developer portal for developers. They can
    + Read docs.
    + Try out API via interactive console.
    + Create an account and subscribe to get API Keys.
    + Access analytics on their own usage.

## Concepts

**API**
A set of operation available to developers. contains a reference to the back-end service and its operations map to the operations implemented by the back-end system.
One can control at the API or operation level:
1. Url Mapping
2. Query and path parameters
3. Request and response content
4. Caching
5. Rate limit
6. Quotas
7. IP restrictions

**Products**
Products are how APIs area surfaced by developers they one or more APIs, and are configured with:
1. Title
2. Description
3. Terms of use
4. Open or protected
   1. Protected. Must be subscribed to before thay can be used.
   2. Open. Can be used without subscription.
5. Subscription approval. administrator aproval || auto-approved

**Groups**
Are used to managed visibility of products to developers
#!Me quedo aqui en los tipos de grupos!

**Developers**

**Policies**


## How to create APIs

## How add operations to an API

## Links

+ [Introduction](https://docs.microsoft.com/en-us/azure/api-management/api-management-key-concepts)
+ [Research white paper](https://j.mp/ms-apim-whitepaper)
+ [How to create](https://docs.microsoft.com/en-us/azure/api-management/api-management-howto-create-apis)
+ [How to add operations](https://docs.microsoft.com/en-us/azure/api-management/api-management-howto-add-operations)

