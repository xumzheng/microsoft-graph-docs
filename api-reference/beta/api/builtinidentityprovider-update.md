---
title: "Update builtInIdentityProvider"
description: "Update the properties of a builtInIdentityProvider object."
author: "IoanPana"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: apiPageType
---

# Update builtInIdentityProvider
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [builtInIdentityProvider](../resources/builtinidentityprovider.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|IdentityProvider.Read.All, IdentityProvider.ReadWrite.All|
|Delegated (personal Microsoft account)|Not supported.|
|Application|IdentityProvider.Read.All, IdentityProvider.ReadWrite.All|

The work or school account needs to belong to one of the following roles:

* Global Administrator
* External Identity Provider Administrator
* External ID user flow administrator

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
In the request body, provide a JSON object with one or more properties that need to be updated for an [identityProvider](../resources/identityprovider.md).


|Property|Type|Description|
|:---|:---|:---|
|displayName|String|The display name of the identity provider. Optional.|
|identityProviderType|String|The type name of the identity provider. Optional.|
|state|identityProviderState|The state value of the identity provider.. The possible values are: `enabled`, `disabled`, `unknownFutureValue`. Optional.|

The work or school account needs to be Global Administrator.


## Response

If successful, this method returns a `200 OK` response code.

## Examples

### Request
The following is an example of a request.
<!-- {
  "blockType": "request",
  "name": "update_builtinidentityprovider"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/builtInIdentityProvider/MSASignup-OAUTH
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
```

