---
title: "Get cloudPcActionStatus"
description: "Read the properties and relationships of a specific cloudPcActionStatus object."
author: "AshleyYangSZ"
ms.localizationpriority: medium
ms.prod: "cloud-pc"
doc_type: apiPageType
---

# Get cloudPcActionStatus

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of a specific [cloudPcActionStatus](../resources/cloudpcactionstatus.md) object.

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

To get the specified [cloudPcActionStatus](../resources/cloudpcactionstatus.md) in the organization, using either delegated permission (the signed-in user should be the administrator) or application permission:

``` http
GET /deviceManagement/virtualEndpoint/cloudPcActionstatuses/{id}
```

## Optional query parameters

This method supports the `$select` OData query parameter to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers

| Name          | Description               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}. Required. |

## Request body

Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [cloudPcActionStatus](../resources/cloudpcactionstatus.md) object in the response body.

## Examples

### Example 1: Get the default properties of a Cloud PC action status

#### Request

The following is an example of a request.


# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpcactionstatus_default_properties"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/cloudPcActionStatuses/662009bc-7732-4f6f-8726-25883518b33e
```
---

#### Response

The following is an example of the response.

<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "get_cloudpcactionstatus_default_properties",
  "@odata.type": "microsoft.graph.cloudPcActionStatus"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.cloudPcActionStatus",
    "id": "662009bc-7732-4f6f-8726-25883518b33e",
    "cloudPcDeviceDisplayName": "CloudPC-Connie",
    "bulkActionId": "bdc8e6dd-0455-4412-83d9-c818664fe1f1",
    "bulkActionDisplayName": null,
    "cloudPcId": "bdc8e6dd-0455-4412-83d9-c818664fe1f1",
    "initiatedByUserPrincipalName": "john@cpccustomer001.onmicrosoft.com",
    "deviceOwnerUserPrincipalName": "connie@cpccustomer001.onmicrosoft.com",
    "action": "Rename",
    "actionState": "failed",
    "requestDateTime": "2020-07-23T10:10:57Z",
    "lastUpdatedDateTime": "2020-07-23T10:29:57Z"
}
```

### Example 2: Get the selected properties of a Cloud PC

#### Request

The following is an example of a request.


# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpcactionstatus_selected_properties"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/cloudPcActionStatuses/662009bc-7732-4f6f-8726-25883518b33e?$select=id,action,actionState,statusDetails
```
---

#### Response

The following is an example of the response.

<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "get_cloudpcactionstatus_selected_properties",
  "@odata.type": "microsoft.graph.cloudPcActionStatus"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.cloudPcActionStatus",
    "id": "662009bc-7732-4f6f-8726-25883518b33e",
    "action": "Rename",
    "actionState": "done",
    "statusDetails": null
}
```
