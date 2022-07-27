---
title: "userFlowPageLayout: availableVersions"
description: "Show page layout versions so developers and can know the available and supported versions."
author: "almars"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: apiPageType
---

# userFlowPageLayout: availableVersions
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

This function is bound only to "userFlowPageLayout" entities with the purpose to show the supported version for page layout, similar to the behavior used in Azure portal when trying to change the version, this with the intention to show developers and admins the exact values allowed to use for a page layout version.

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
GET /identity/b2cUserFlows/{b2cIdentityUserFlowId}/pageLayouts/{userFlowPageLayoutId}/availableVersions
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this function returns a `200 OK` response code and a String collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "userflowpagelayoutthis.availableversions"
}
-->
``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{b2cIdentityUserFlowId}/pageLayouts/{userFlowPageLayoutId}/availableVersions
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Edm.String)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    "String"
  ]
}
```

