---
title: "Update builtInIdentityProvider"
description: "Update the properties of a builtInIdentityProvider object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
doc_type: apiPageType
---

# Update builtInIdentityProvider
Namespace: microsoft.graph



Update the properties of a [builtInIdentityProvider](../resources/builtinidentityprovider.md) object.

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
PATCH /builtInIdentityProvider
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
|displayName|String|**TODO: Add Description** Inherited from [identityProviderBase](../resources/identityproviderbase.md). Optional.|
|identityProviderType|String|**TODO: Add Description** Optional.|
|state|identityProviderState|**TODO: Add Description**. The possible values are: `enabled`, `disabled`, `unknownFutureValue`. Optional.|



## Response

If successful, this method returns a `200 OK` response code and an updated [builtInIdentityProvider](../resources/builtinidentityprovider.md) object in the response body.

## Examples

### Request
The following is an example of a request.
<!-- {
  "blockType": "request",
  "name": "update_builtinidentityprovider"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/builtInIdentityProvider
Content-Type: application/json
Content-length: 152

{
  "@odata.type": "#microsoft.graph.builtInIdentityProvider",
  "displayName": "String",
  "identityProviderType": "String",
  "state": "String"
}
```


### Response
The following is an example of the response
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
  "@odata.type": "#microsoft.graph.builtInIdentityProvider",
  "id": "84f8e568-3552-a74d-bb3e-634f3c9a5342",
  "displayName": "String",
  "identityProviderType": "String",
  "state": "String"
}
```

