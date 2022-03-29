---
title: "alertRecord: getPortalNotifications"
description: "View a list of all portal notifications that are ready to be consumed for current user. The portal notifications can be used to publish MEM portal notifications."
author: "zhishending"
ms.localizationpriority: medium
ms.prod: "cloud-pc"
doc_type: apiPageType
---

# alertRecord: getPortalNotifications
Namespace: microsoft.graph.deviceManagement

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

View a list of all portal notifications that are ready to be consumed for current user. The portal notifications can be used to publish MEM portal notifications.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|CloudPC.ReadWrite.All|
|Delegated (work or school account)|CloudPC.Read.All|
|Delegated (personal Microsoft account)|Not supported.|
|Application|CloudPC.ReadWrite.All|
|Application|CloudPC.Read.All|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/monitoring/alertRecords/getPortalNotifications
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this function returns a `200 OK` response code and a [microsoft.graph.deviceManagement.portalNotification](../resources/devicemanagement-portalnotification.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "alertrecordthis.getportalnotifications"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/monitoring/alertRecords/getPortalNotifications
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.deviceManagement.portalNotification)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "microsoft.graph.deviceManagement.portalNotification"
    }
  ]
}
```
