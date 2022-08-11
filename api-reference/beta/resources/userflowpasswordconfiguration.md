---
title: "userFlowPasswordConfiguration resource type."
description: "API doc to provide details on the password configuration for a b2c userflow"
author: "harsh-aseeja"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: resourcePageType
---

# userFlowPasswordConfiguration resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## Password Configration options

Password complexity can be configured in the following types of user flows:

- Sign-up or Sign-in user flow
- Password Reset user flow

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowExpiredPasswordReset|Boolean| If `true`, allows end users with expired passwords to reset their password |
|complexityLevel|userFlowPasswordComplexityLevel|The possible values are: `simple`, `strong`, `custom`.|
|customConfiguration|[userFlowCustomPasswordComplexity](../resources/userflowcustompasswordcomplexity.md)|Provides ability to set a custom password complexity|
|isSelfServicePasswordResetAllowed|Boolean|If this is set to `true`, then this userflow will also support self service password reset without needing another password reset userflow.|

### userFlowPasswordComplexityLevel values
|Value|Description|
|:---|:---|
|simple|A password that is at least 8 to 64 characters.|
|strong|A password that is at least 8 to 64 characters. It requires 3 out of 4 of lowercase, uppercase, numbers, or symbols.|
|custom|This option provides the most control over password complexity rules. It allows configuring a custom length. It also allows accepting number-only passwords (pins).  [userFlowCustomPasswordComplexity](../resources/userflowcustompasswordcomplexity.md)|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userFlowPasswordConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userFlowPasswordConfiguration",
  "isSelfServicePasswordResetAllowed": "Boolean",
  "allowExpiredPasswordReset": "Boolean",
  "complexityLevel": "String",
  "customConfiguration": {
    "@odata.type": "microsoft.graph.userFlowCustomPasswordComplexity"
  }
}
```

