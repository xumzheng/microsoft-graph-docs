---
title: "Get eaAppPerformance"
description: "Read the properties and relationships of an eaAppPerformance object."
author: "idwilliams"
ms.localizationpriority: medium
ms.prod: "microsoft-365-lighthouse"doc_type: apiPageType
---

# Get eaAppPerformance
Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of an [eaAppPerformance](../resources/managedtenants-eaappperformance.md) object.

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
GET /managedTenant/eaAppPerformances/{eaAppPerformanceId}
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

If successful, this method returns a `200 OK` response code and an [eaAppPerformance](../resources/managedtenants-eaappperformance.md) object in the response body.

## Examples

### Request
The following is an example of a request.
<!-- {
  "blockType": "request",
  "name": "get_eaappperformance"
}
-->
``` http
GET https://graph.microsoft.com/beta/managedTenant/eaAppPerformances/{eaAppPerformanceId}
```


### Response
The following is an example of the response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.eaAppPerformance"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.managedTenants.eaAppPerformance",
    "id": "a92a7b20-eebf-b244-efeb-7101a6dc288b",
    "appName": "String",
    "appFriendlyName": "String",
    "appPublisher": "String",
    "tenantId": "String",
    "tenantDisplayName": "String",
    "totalActiveDeviceCount": "Integer",
    "totalAppCrashCount": "Integer",
    "totalAppFreezeCount": "Integer",
    "meanTimeToFailureInMinutes": "Integer",
    "lastUpdatedDateTime": "String (timestamp)"
  }
}
```

