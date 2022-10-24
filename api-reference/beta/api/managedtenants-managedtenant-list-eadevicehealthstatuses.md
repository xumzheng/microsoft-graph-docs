---
title: "List eaDeviceHealthStatus"
description: "Get a list of the eaDeviceHealthStatus objects and their properties."
author: "idwilliams"
ms.localizationpriority: medium
ms.prod: "microsoft-365-lighthouse"doc_type: apiPageType
---

# List eaDeviceHealthStatus
Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the [eaDeviceHealthStatus](../resources/managedtenants-eadevicehealthstatus.md) objects and their properties.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /managedTenant/eaDeviceHealthStatuses
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [eaDeviceHealthStatus](../resources/eadevicehealthstatus.md) objects in the response body.

## Examples

### Request
The following is an example of a request.
<!-- {
  "blockType": "request",
  "name": "list_eadevicehealthstatus"
}
-->
``` http
GET https://graph.microsoft.com/beta/managedTenant/eaDeviceHealthStatuses
```


### Response
The following is an example of the response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.eaDeviceHealthStatus)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedTenants.eaDeviceHealthStatus",
      "id": "2bc015f6-9f6e-9342-01f1-9abebb2d05c9",
      "tenantId": "String",
      "tenantDisplayName": "String",
      "deviceId": "String",
      "deviceName": "String",
      "deviceModel": "String",
      "deviceMake": "String",
      "osVersion": "String",
      "primaryDiskType": "String",
      "startupPerformanceScore": "Double",
      "bootTotalDurationInSeconds": "Double",
      "restartCount": "Integer",
      "blueScreenCount": "Integer",
      "healthStatus": "String",
      "topProcesses": "String",
      "lastUpdatedDateTime": "String (timestamp)"
    }
  ]
}
```

