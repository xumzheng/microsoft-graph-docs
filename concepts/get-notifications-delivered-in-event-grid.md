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

Follow the steps in [subscribe to partner events](https://docs.microsoft.com/en-us/azure/event-grid/subscribe-to-partner-events) to start receiving events from any of the event sources supported by Microsoft Graph API.

## Need help?

We are here to help you. If you have questions of the use of Azure Graph API with Event Grid, please send us an email to <a href="mailto:ask.graph.and.grid@service.microsoft.com">mailto:ask.graph.and.grid@service.microsoft.com</a>
