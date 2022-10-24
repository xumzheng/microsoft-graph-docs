---
title: "List eaAppPerformances"
description: "Get a list of the eaAppPerformance objects and their properties."
author: "idwilliams"
ms.localizationpriority: medium
ms.prod: "microsoft-365-lighthouse"doc_type: apiPageType
---

# List eaAppPerformances
Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the [eaAppPerformance](../resources/managedtenants-eaappperformance.md) objects and their properties.

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
GET /managedTenant/eaAppPerformances
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

If successful, this method returns a `200 OK` response code and a collection of [eaAppPerformance](../resources/eaappperformance.md) objects in the response body.

## Examples

### Request
The following is an example of a request.
<!-- {
  "blockType": "request",
  "name": "list_eaappperformance"
}
-->
``` http
GET https://graph.microsoft.com/beta/managedTenant/eaAppPerformances
```


### Response
The following is an example of the response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.eaAppPerformance)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
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
  ]
}
```

