---
title: "List pageLayouts associated to a userflow"
description: "Get the list of page layouts in a userflow."
author: "almars"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: apiPageType
---

# List userFlowPageLayouts
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get the pageLayouts in an userflow. Userflow pageLayouts are represented by the [userFlowPageLayout](../resources/userflowpagelayout.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All|
|Delegated (personal Microsoft account)|Not supported.|
|Application|IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identity/b2cUserFlows/{b2cIdentityUserFlowId}/pageLayouts
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

If successful, this method returns a `200 OK` response code and a collection of [userFlowPageLayout](../resources/userflowpagelayout.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_userflowpagelayout"
}
-->
``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/b2cUserFlows/B2C_1_Example/pageLayouts
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userFlowPageLayout)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Example/pageLayouts/",
    "value": [
      {
      "id": "api.signinandsignupwithpassword1.1",
      "displayName": "Unified sign up or sign in page",
      "isCustomPageUri": "false",
      "pageUri": "https://authxcustomizationb2c.onmicrosoft.com/static/tenant/templates/AzureBlue/unified.cshtml",
      "version": "2.1.1"
      },
      {
      "id": "api.selfasserted.expiredpassword",
      "displayName": "Update expired password page",
      "isCustomPageUri": "false",
      "pageUri": "https://authxcustomizationb2c.onmicrosoft.com/static/tenant/templates/AzureBlue/selfAsserted.cshtml",
      "version": "2.1.1"
      }
    ]
}
```

