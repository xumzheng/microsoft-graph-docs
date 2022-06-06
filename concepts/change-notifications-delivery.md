---
title: "Get change notifications delivered in different ways"
description: "Change notifications can be delivered via different technologies, including webhooks and Azure Event Hubs."
author: "Jumaodhiss"
ms.localizationpriority: high
ms.custom: graphiamtop20, devx-track-azurecli
---

# Get change notifications delivered in different ways

Change notifications can be delivered in different ways to subscribers. If the main delivery mode for change notifications is through webhooks, it can be challenging to take advantage of webhooks for high throughput scenarios or when the receiver cannot expose a publicly available notification URL.  

These change notifications delivery modes are available for all resources that support Microsoft Graph change notifications.

Good examples of high throughput scenarios include applications subscribing to a large set of resources, applications subscribing to resources that change with a high frequency, and multi-tenant applications that subscribe to resources accross a large set of organizations.