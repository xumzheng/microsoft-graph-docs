---
title: "builtInIdentityProvider resource type"
description: "Represents built-in identity providers in an Azure Active Directory tenant."
author: "namkedia"
ms.localizationpriority: high
ms.prod: "identity-and-sign-in"
doc_type: resourcePageType
---

# builtInIdentityProvider resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents built-in identity providers with [External Identities](/azure/active-directory/external-identities/) for an Azure Active Directory tenant.

For Azure AD B2B scenarios in an Azure AD tenant, the built in identity provider type can be an Azure Active Directory(AAD), Microsoft account(MSA) or email one-time passcode (EmailOTP).

Inherits from [identityProviderBase](../resources/identityproviderbase.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List builtInIdentityProviders](../api/builtinidentityprovider-list.md)|[builtInIdentityProvider](../resources/builtinidentityprovider.md) collection|Get a list of the [builtInIdentityProvider](../resources/builtinidentityprovider.md) objects and their properties.|
|[Get builtInIdentityProvider](../api/builtinidentityprovider-get.md)|[builtInIdentityProvider](../resources/builtinidentityprovider.md)|Read the properties and relationships of a [builtInIdentityProvider](../resources/builtinidentityprovider.md) object.|
|[Update builtInIdentityProvider](../api/builtinidentityprovider-update.md)|[builtInIdentityProvider](../resources/builtinidentityprovider.md)|Update the properties of a [builtInIdentityProvider](../resources/builtinidentityprovider.md) object (only MSA).|
|[Delete builtInIdentityProvider](../api/builtinidentityprovider-delete.md)|None|Deletes a [builtInIdentityProvider](../resources/builtinidentityprovider.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description** Inherited from [identityProviderBase](../resources/identityproviderbase.md).|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|identityProviderType|String|**TODO: Add Description**|
|state|identityProviderState|**TODO: Add Description**.The possible values are: `enabled`, `disabled`, `unknownFutureValue`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.builtInIdentityProvider",
  "baseType": "microsoft.graph.identityProviderBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.builtInIdentityProvider",
  "id": "String (identifier)",
  "displayName": "String",
  "identityProviderType": "String",
  "state": "String"
}
```

