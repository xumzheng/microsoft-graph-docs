---
title: "Get eaDeviceAppPerformance"
description: "Read the properties and relationships of an eaDeviceAppPerformance object."
author: "idwilliams"
ms.localizationpriority: medium
ms.prod: "microsoft-365-lighthouse"doc_type: apiPageType
---

# Get eaDeviceAppPerformance
Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of an [eaDeviceAppPerformance](../resources/managedtenants-eadeviceappperformance.md) object.

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
GET /managedTenant/eaDeviceAppPerformances/{eaDeviceAppPerformanceId}
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

If successful, this method returns a `200 OK` response code and an [eaDeviceAppPerformance](../resources/managedtenants-eadeviceappperformance.md) object in the response body.

## Examples

### Request
The following is an example of a request.
<!-- {
  "blockType": "request",
  "name": "get_eadeviceappperformance"
}
-->
``` http
GET https://graph.microsoft.com/beta/managedTenant/eaDeviceAppPerformances/{eaDeviceAppPerformanceId}
```


### Response
The following is an example of the response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.eaDeviceAppPerformance"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.managedTenants.eaDeviceAppPerformance",
    "id": "51515139-9b32-6132-1371-f7556350b011",
    "appName": "String",
    "appFriendlyName": "String",
    "appPublisher": "String",
    "appVersion": "String",
    "tenantId": "String",
    "tenantDisplayName": "String",
    "deviceId": "String",
    "deviceName": "String",
    "deviceModel": "String",
    "deviceManufacturer": "String",
    "healthStatus": "String",
    "totalAppCrashCount": "Integer",
    "totalAppFreezeCount": "Integer",
    "isLatestUsedVersion": "Integer",
    "isMostUsedVersion": "Integer",
    "lastUpdatedDateTime": "String (timestamp)"
  }
}
```

