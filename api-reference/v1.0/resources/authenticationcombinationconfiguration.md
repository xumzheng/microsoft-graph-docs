---
title: "authenticationCombinationConfiguration resource type"
description: "An abstract configuration for a given auth method applied to certain combinations. "
author: "InbarckMS"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: resourcePageType
---

# authenticationCombinationConfiguration resource type

Namespace: microsoft.graph

An authentication combination configuration sets restrictions on specific types, modes, and versions of an authentication method that is tied to specific auth method combinations used in an [authentication strength](authenticationstrengths-overview.md).
This is an abstract type. In use, [fido2combinationConfigurations](fido2combinationconfiguration.md) may be created and managed as described below.


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List authenticationCombinationConfigurations](../api/authenticationstrengthpolicy-list-combinationconfigurations.md)|[authenticationCombinationConfiguration](../resources/authenticationcombinationconfiguration.md) collection|Get a list of the [authenticationCombinationConfiguration](../resources/authenticationcombinationconfiguration.md) objects and their properties.|
|[Create authenticationCombinationConfiguration](../api/authenticationstrengthpolicy-post-combinationconfigurations.md)|[authenticationCombinationConfiguration](../resources/authenticationcombinationconfiguration.md)|Create a new [authenticationCombinationConfiguration](../resources/authenticationcombinationconfiguration.md) object.|
|[Get authenticationCombinationConfiguration](../api/authenticationcombinationconfiguration-get.md)|[authenticationCombinationConfiguration](../resources/authenticationcombinationconfiguration.md)|Read the properties and relationships of an [authenticationCombinationConfiguration](../resources/authenticationcombinationconfiguration.md) object.|
|[Update authenticationCombinationConfiguration](../api/authenticationcombinationconfiguration-update.md)|[authenticationCombinationConfiguration](../resources/authenticationcombinationconfiguration.md)|Update the properties of an [authenticationCombinationConfiguration](../resources/authenticationcombinationconfiguration.md) object.|
|[Delete authenticationCombinationConfiguration](../api/authenticationstrengthpolicy-delete-combinationconfigurations.md)|None|Delete an [authenticationCombinationConfiguration](../resources/authenticationcombinationconfiguration.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appliesToCombinations|authenticationMethodModes collection|Which authentication method combinations this configuration applies to. Must be an **allowedCombinations** object that's defined for the [authenticationStrengthPolicy](../resources/authenticationstrengthpolicy.md). The only possible value for fido2combinationConfigurations is `"fido2"`.|
|id|String|A unique system-generated identifier. Inherited from [entity](../resources/entity.md).|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationCombinationConfiguration",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationCombinationConfiguration",
  "id": "String (identifier)",
  "appliesToCombinations": [
    "String"
  ]
}
```

