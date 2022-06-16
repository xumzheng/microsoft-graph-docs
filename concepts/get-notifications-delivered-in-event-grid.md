---
title: "Get change notifications delivered in different ways"
description: "Change notifications can be delivered via different technologies, including webhooks and Azure Event Hubs."
author: "Jumaodhiss, jafernan"
ms.localizationpriority: high
ms.custom: graphiamtop20, devx-track-azurecli, azure-event-grid, event-grid, pubsub
---

# Using Azure Event Grid to receive change notifications (Preview)

[Azure Event Grid](https://docs.microsoft.com/en-us/azure/event-grid/compare-messaging-services#azure-event-grid)Event Grid is a highly scalable, serverless event broker you can use to integrate applications using event-driven architectures. Microsoft Graph API can send notifications to Event Grid in the form of [CloudEvents](https://github.com/cloudevents/spec/blob/v1.0.2/cloudevents/spec.md) announcing state changes to [supported Microsoft Graph API resources](https://docs.microsoft.com/en-us/graph/webhooks?view=graph-rest-1.0#supported-resources). The event types that are raised when there is a state change in those resources are described in the following articles:

1. [Azure AD events](https://docs.microsoft.com/en-us/azure/event-grid/azure-active-directory-events)
2. [Microsoft Outlook events](https://docs.microsoft.com/en-us/azure/event-grid/outlook-events)

The Event Grid feature that enables Microsoft Graph API to send events to Event Grid is [Partner Events](partner-events-overview.md).

## Receive events on Microsoft Graph API resource state changes on Event Grid

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

Follow the steps in [subscribe to partner events](https://docs.microsoft.com/en-us/azure/event-grid/subscribe-to-partner-events) to start receiving events from any of the event sources supported by Microsoft Graph API.

## Need help?

We are here to help you. If you have questions of the use of Azure Graph API with Event Grid, please send us an email to <a href="mailto:ask.graph.and.grid@service.microsoft.com">mailto:ask.graph.and.grid@service.microsoft.com</a>
