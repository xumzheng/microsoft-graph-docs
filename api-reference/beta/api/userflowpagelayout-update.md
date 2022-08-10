---
title: "Update userflowPageLayout"
description: "Update a page layout in a user flow."
author: "almars"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: apiPageType
---

# Update userflowPageLayout
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update a [page layout](../resources/userflowpagelayout.md) in an userflow.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|IdentityUserFlow.ReadWrite.All|
|Delegated (personal Microsoft account)|Not supported.|
|Application|IdentityUserFlow.ReadWrite.All|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /identity/b2cUserFlows/{b2cIdentityUserFlowId}/pageLayouts/{userFlowPageLayoutId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|Property|Type|Description|
|:---|:---|:---|
|pageUri|String|Location for the ".html" resource used to load the custom content, as show in [documentation](https://docs.microsoft.com/azure/active-directory-b2c/customize-ui-with-html?pivots=b2c-user-flow#4-update-the-user-flow). Optional.|
|version|String|Version of the page layout. Optional.|



## Response

If successful, this method returns a `200 OK` response code and an updated [userFlowPageLayout](../resources/userflowpagelayout.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_userflowpagelayout"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Example/pageLayouts/api.signinandsignupwithpassword1.1
Content-Type: application/json
Content-length: 169

{
  "@odata.type": "#microsoft.graph.userFlowPageLayout",
  "displayName": "String",
  "isCustomPageUri": "Boolean",
  "pageUri": "String",
  "version": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Example/pageLayouts/"
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

