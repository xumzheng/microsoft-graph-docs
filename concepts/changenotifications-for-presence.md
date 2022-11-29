---
title: "Get change notifications for Microsoft Teams Presence updates"
description: "Use change notifications in Microsoft Graph to enable you to subscribe to Microsoft Teams Presence updates."
author: "satyakonmsft"
ms.localizationpriority: high
ms.prod: "cloud-communications"
ms.custom: scenarios:getting-started
---

# Get change notifications for Microsoft Teams Presence updates

Change notifications in Microsoft Graph enable you to subscribe to the Teams presence information of your own and other users. Change notifications provide a low-latency model by allowing you to maintain a subscription. You can also get the resource data in the notifications and therefore avoid calling the API to get the payload.
This is an alternative to polling for presence by using the [GET presence](../api-reference/v1.0/api/presence-get) and [POST getPresencesByUserId](../api-reference/v1.0/api/cloudcommunications-getpresencesbyuserid) APIs.

1. Subscribe to a single user’s presence through the /communications/presences/{id} path.

2. Subscribe to a maximum number of 650 users by using /communications/presences?$filter=id in ({id},{id}...). The {id} represents a user ID GUID.

Subscriptions expire every hour and must be renewed.

This resource supports notifications with resource data. For more information about setting up notifications with resource data, see [Set up change notifications that include resource data](/graph/webhooks-with-resource-data).

### Permissions

|Permission type      | Permissions (from least to most privileged)              | Supported versions |
|:--------------------|:---------------------------------------------------------|:-------------------|
|Delegated (work or school account) | Presence.Read.All. | v1.0, beta |
|Delegated (personal Microsoft account) | Not supported.    | Not supported. |
|Application | Not supported. | Not supported. |

### Example

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/communications/presences/{id}",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2021-02-01T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

> [!NOTE]
> Replace `{id}` with the actual user's AAD objectid when specifying the resource.

## Notifications with encrypted resource data

```json
{
  "value": [{
    "subscriptionId": "{Subscription id}",
    "clientState": "{secret client state}",
    "changeType": "updated",
    "tenantId": "{Organization/Tenant id}",
    "resource": "/communications/presences/{id}",
    "subscriptionExpirationDateTime": "2022-02-28T00:00:00.0000000Z",
    "resourceData": {
      "@odata.id": "/communications/presences/{id}",
      "@odata.type": "#microsoft.graph.presence",
      "id": "/communications/presences/{id}"
    },
    "organizationId": "{Organization/Tenant id}",
    "encryptedContent": {
      "data": "{Encrypted content}",
      "dataSignature": "{Encrypted data signature}",
      "dataKey": "{Encrypted data key for encrypting content}",
      "encryptionCertificateId": "{User specified id of encryption certificate}",
      "encryptionCertificateThumbprint": "{Encrpytion certification thumbprint}"
    }
  }],
  "validationTokens": ["{Validation Tokens}"]
}
```

For details about how to validate tokens and decrypt the payload, see [Set up change notifications that include resource data](/graph/webhooks-with-resource-data).

### Decrypted payload examples

#### Single User Presence Updated
```json
{
  "@odata.type":"#Microsoft.Graph.presence",
  "@odata.id":"/communications/presences/{id}",
  "id":"/communications/presences/{id}",
  "activity":"Busy",
  "availability":"Busy"
}

```
#### Multiple User Presence Updated
```json
{
  "@odata.type":"#Microsoft.Graph.presence",
  "@odata.id":"/communications/presences/{id}",
  "id":"/communications/presences/{id}",
  "activity":"Busy",
  "availability":"Busy"
}
```

## See also

- [Microsoft Graph change notifications](/graph/webhooks)
- [Microsoft Teams API overview](/graph/teams-concept-overview)
- [Presence resource](/graph/api/resources/presence)
