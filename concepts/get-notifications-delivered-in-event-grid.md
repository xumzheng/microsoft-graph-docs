---
title: "Get change notifications delivered in different ways"
description: "Change notifications can be delivered via different technologies, including webhooks and Azure Event Hubs."
author: "Jumaodhiss"
ms.localizationpriority: high
ms.custom: graphiamtop20, devx-track-azurecli
---

# Using Azure Event Grid to receive change notifications (Preview)

[Azure Event Grid](https://docs.microsoft.com/en-us/azure/event-grid/compare-messaging-services#azure-event-grid) is an eventing backplane that enables event-driven, reactive programming. It uses the publish-subscribe model. Publishers emit events, but have no expectation about how the events are handled. Subscribers decide on which events they want to handle.

Today third-party SaaS providers use Azure event grid partner topics to publish events from its services so that their customers can subscribe to those events.  

This feature enables Microsoft Graph change notifications to be delivered via Azure event grid partner topics. SaaS provides and their customers can subscribe to Microsoft graph change notifications [supported resources](https://docs.microsoft.com/en-us/graph/api/resources/webhooks?view=graph-rest-1.0) to be delivered through Azure Event Grid partner topics

## Configuring the Azure Event Grid

In this section we will walk you through how to setup an Azure Event Grid partner topic that you can use to receive Microsoft Graph change notifications.

### Enable Azure Event Grid Resource Provider

If you haven't previously used Azure Event Grid in your Azure subscription, you need to register the Event Grid resource provider. Please follow [these steps](https://docs.microsoft.com/en-us/azure/event-grid/custom-event-quickstart-portal#enable-event-grid-resource-provider) to register Azure Event Grid resource provider in your Azure subscription
### Authorize Microsoft Graph to create partner topic
You must grant your consent to Microsoft Graph to create partner topics in your resource group. This authorization has an expiration time. It's effective for the time period you specify between 1 to 365 days. To consent follow the [these steps](https://docs.microsoft.com/en-us/azure/event-grid/subscribe-to-partner-events#authorize-partner-to-create-a-partner-topic)
### Creating Microsoft Graph Subscription
Creating subscriptions to Microsoft graph change notifications with Event grid is similar to creating subscription to change notifications delivered via webhooks. The key difference is that there is need to specify the Event Grid partner topic properties. All other operations are similar, including [subscription creation](/graph/api/subscription-post-subscriptions).

The main difference during subscription creation is the **notificationUrl** property in the request payload. You must set it to `EventGrid:?azuresubscriptionid=<azuresubscriptionid>&resourcegroup=<resourcegroup>&partnertopic=<partnertopic>&location=<location>`, with the following values:

- `azuresubscriptionid` - The azure subscription id where the customer (subscriber) wishes to creates the partner topic to receive microsoft graph changes notifications.
- `resourcegroup` - The Azure resource group where the customer (subscriber) wishes to creates the partner topic to receive microsoft graph changes notifications. creates the partner topic to receive changes notifications.
- `partnertopic` - The customer's preferred event grid partner topic name. The system automatically verifies whether the partner topic exists. A new partner topic is created if it doesn't exist
- `location` - The location where the customer (subscriber) wishes to creates the partner topic to receive microsoft graph changes notifications.

> **Note:** Partner topic name must be unique within the same region. Both Microsoft Graph and Azure Event grid enforces the uniqueness of partner topics. Each tenant together with each application may create up to 10 unique partner topics.

#### Subscription request example
The following example subscribes to users being updated or deleted
```json
{
    "changeType": "Updated,Deleted",
    "notificationUrl": "EventGrid:?azuresubscriptionid=<id>&resourcegroup=<rg>&partnertopic=<topic>&location=<location>",
    "resource": "Users",
    "expirationDateTime": "<subscription-expiration-time>",
    "clientState": "mysecret"
}
```
#### Subscription creation response
```json
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscriptions/$entity",
    "id": "<subscriptionid>",
    "resource": "users",
    "applicationId": "<application id>",
    "changeType": "updated,deleted",
    "clientState": "mysecret",
    "notificationUrl": "EventGrid:?azuresubscriptionid=<id>&resourcegroup=<rg>&partnertopic=<topic>",
    "blobStoreUrl": null,
    "lifecycleNotificationUrl": null,
    "expirationDateTime": "2022-04-07T20:30:00Z",
    "creatorId": "<creator id>",
    "includeProperties": null,
    "includeResourceData": null,
    "latestSupportedTlsVersion": null,
    "encryptionCertificate": null,
    "encryptionCertificateId": null,
    "notificationUrlAppId": null
}
```
#### Activating partner topics
When the subscription is created successfully, an event grid partner topic is automatically created. The partner topic is inactive by default therefore you (the customer) must login to your azure subscription and activate it. To activate a partner topic follow [these steps](/azure/event-grid/subscribe-to-partner-events#activate-a-partner-topic)

#### Adding event subscription
When the partner topic receives a notification from microsoft graph, the notifications is forwarded to the customer preferred endpoint. To register the end point, you need to add an event subscription to your partner topic. Follow the steps to [create event subscription](/azure/event-grid/subscribe-to-partner-events#subscribe-to-events)