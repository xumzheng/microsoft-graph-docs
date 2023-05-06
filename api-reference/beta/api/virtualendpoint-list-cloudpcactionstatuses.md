---
title: "List cloudPcActionStatuses"
description: "List properties and relationships of the cloudPC objects."
author: "AshleyYangSZ"
ms.localizationpriority: medium
ms.prod: "cloud-pc"
doc_type: apiPageType
---

# List cloudPcActionStatuses

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

List the [cloudPcActionStatus](../resources/cloudpcactionstatus.md) device action status in a tenant.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|CloudPC.Read.All, CloudPC.ReadWrite.All|
|Delegated (personal Microsoft account)|Not supported.|
|Application|CloudPC.Read.All, CloudPC.ReadWrite.All|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/cloudPcActionStatuses
```

## Optional query parameters

This method supports `$select`, `$filter`, `@odata.nextLink` and `$count` OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers

| Name          | Description               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}. Required. |

## Request body

Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [cloudPcActionStatus](../resources/cloudpcactionstatus.md) objects in the response body.

## Examples

### Request


# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpcactionstatuses"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/actionStatuses?$count=true&top=200
```
---

### Response

**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.cloudPcActionStatus)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#deviceManagement/virtualEndpoint/$metadata#cloudPcActionStatuses",    
    "@odata.count": 377,
    "@odate.nextLink": "https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/actionStatuses?$count=true&top=200&$skip=200",
    "value": [
        {
            "id": "662009bc-7732-4f6f-8726-25883518b33e",
            "cloudPcDeviceDisplayName": "CloudPC-Connie",
            "bulkActionId": "bdc8e6dd-0455-4412-83d9-c818664fe1f1",
            "bulkActionDisplayName": "Resize to 64GB RAM - John",
            "cloudPcId": "bdc8e6dd-0455-4412-83d9-c818664fe1f1",
            "initiatedByUserPrincipalName": "john@cpccustomer001.onmicrosoft.com",
            "deviceOwnerUserPrincipalName": "connie@cpccustomer001.onmicrosoft.com",
            "action": "Resize",
            "actionState": "failed",
            "requestDateTime": "2020-07-23T10:10:57Z",
            "lastUpdatedDateTime": "2020-07-23T10:29:57Z"
        },
        {
            "id": "ac74ae8b-85f7-4272-88cc-5419267403ed",
            "cloudPcDeviceDisplayName": "CloudPC-Brian",
            "bulkActionId": "bdc8e6dd-0455-4412-83d9-c818664fe1f1",
            "bulkActionDisplayName": "Resize to 64GB RAM - John",
            "cloudPcId": "e87f50c7-fa7f-4687-aade-dd45f3d65970",
            "initiatedByUserPrincipalName": "john@cpccustomer001.onmicrosoft.com",
            "deviceOwnerUserPrincipalName": "brian@cpccustomer001.onmicrosoft.com",
            "action": "Resize",
            "actionState": "done",
            "requestDateTime": "2020-07-23T10:10:57Z",
            "lastUpdatedDateTime": "2020-07-23T10:29:57Z"
        },
        {
            "id": "cabe9575-2d7f-4741-a9a9-86be71643a67",
            "cloudPcDeviceDisplayName": "CloudPC-Brian",
            "bulkActionId": "bdc8e6dd-0455-4412-83d9-c818664fe1f1",
            "bulkActionDisplayName": "Resize to 64GB RAM - John",
            "cloudPcId": "e87f50c7-fa7f-4687-aade-dd45f3d65970",
            "managedDeviceId": "b9fd17fa-64d5-45b1-86bc-ff928d951fa5",
            "initiatedByUserPrincipalName": "john@cpccustomer001.onmicrosoft.com",
            "deviceOwnerUserPrincipalName": "brian@cpccustomer001.onmicrosoft.com",
            "action": "Resize",
            "actionState": "failed",
            "requestDateTime": "2020-07-25T08:10:57Z",
            "lastUpdatedDateTime": "2020-07-25T08:29:57Z"
        },
        {
            "id": "cabe9575-2d7f-4741-a9a9-86be71643a67",
            "cloudPcDeviceDisplayName": "CloudPC-Mike",
            "bulkActionId": "bdc8e6dd-0455-4412-83d9-c818664fe1f1",
            "bulkActionDisplayName": "Resize to 64GB RAM - John",
            "cloudPcId": "e87f50c7-fa7f-4687-aade-dd45f3d65970",
            "initiatedByUserPrincipalName": "john@cpccustomer001.onmicrosoft.com",
            "deviceOwnerUserPrincipalName": "mike@cpccustomer001.onmicrosoft.com",
            "action": "Resize",
            "actionState": "done",
            "requestDateTime": "2020-07-25T08:10:57Z",
            "lastUpdatedDateTime": "2020-07-25T08:29:57Z"
        }
    ]
}
```
