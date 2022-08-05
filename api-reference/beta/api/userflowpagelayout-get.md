---
title: "Get userFlowPageLayout"
description: "Retrieve a page layout in a b2cidentityuserflow."
author: "almars"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: apiPageType
---

# Get userFlowPageLayout
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Retrieve a [page layout](../resources/userflowpagelayout.md) in a b2cidentityuserflow.

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
GET /identity/b2cUserFlows/B2C_1_Example/pageLayouts/api.signinandsignupwithpassword1.1
```

## Optional query parameters
This method supports $filter OData query parameter to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [userFlowPageLayout](../resources/userflowpagelayout.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_userflowpagelayout"
}
-->
``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Example/pageLayouts/api.signinandsignupwithpassword1.1
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userFlowPageLayout"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.userFlowPageLayout",
    "id": "8073a745-debc-c577-dfc9-e5b451c6b227",
    "displayName": "Unified sign up or sign in page",
    "isCustomPageUri": "false",
    "pageUri": "https://authxcustomizationb2c.onmicrosoft.com/static/tenant/templates/AzureBlue/unified.cshtml",
    "version": "2.1.1"
  }
}
```

