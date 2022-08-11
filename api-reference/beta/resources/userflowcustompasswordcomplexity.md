---
title: "userFlowCustomPasswordComplexity resource type"
description: "API doc to describe custom password complexity"
author: "harsh-aseeja"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: resourcePageType
---

# userFlowCustomPasswordComplexity resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]



## Properties
|Property|Type|Description|
|:---|:---|:---|
|minimumLength|Int32|Minimum Length must be at least 4|
|maximumLength|Int32|Maximum Length must be greater or equal to minimum length and at most can be 256 characters.|
|minimumCharacterClassesRequired|Int32|Allows you to control the different character types used in the password. Possible values are `2`, `3` and `4`|
|restrictToNumbersOnly|Boolean|Numbers only allows digits only (0-9) while entering a password.|

### Character classes

|Value|Description|
|:---|:---|
|2|2 of 4: Lowercase character, Uppercase character, Number (0-9), Symbol ensures the password contains at least two character types. For example, a number and a lowercase character|
|3|3 of 4: Lowercase character, Uppercase character, Number (0-9), Symbol ensures the password contains at least three character types. For example, a number, a lowercase character and an uppercase character.|
|4|4 of 4: Lowercase character, Uppercase character, Number (0-9), Symbol ensures the password contains all  character types.|






## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userFlowCustomPasswordComplexity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userFlowCustomPasswordComplexity",
  "minimumLength": "Integer",
  "maximumLength": "Integer",
  "restrictToNumbersOnly": "Boolean",
  "minimumCharacterClassesRequired": "Integer"
}
```

