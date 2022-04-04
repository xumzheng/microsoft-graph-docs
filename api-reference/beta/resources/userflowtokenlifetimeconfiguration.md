---
title: "userFlowSingleSignOnSessionConfiguration resource type"
description: "Configure the lifetime for ID, access and refresh tokens in Azure AD B2C user flows."
author: "nickgmicrosoft"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: resourcePageType
---


# userFlowTokenLifetimeConfiguration resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Configures the lifetime for ID, access and refresh tokens.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accessAndIdTokenLifetimeInMinutes|Int32| The lifetime of the OAuth 2.0 bearer Id token and access token used to gain access to a protected resource. Default value is 60 minutes. |
|refreshTokenLifetimeInDays|Int32| The maximum time period before which a refresh token can be used to acquire a new access or ID token. Default value is 14 days. |
|rollingRefreshTokenLifetimeInDays|Int32| The time period after which the the user is forced to re-authenticate, irrespective of the validity period of the most recent refresh token acquired by the app. If set to `-1`, the refresh token doesn't expire. Default value is 90 days.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userFlowTokenLifetimeConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userFlowTokenLifetimeConfiguration",
  "accessAndIdTokenLifetimeInMinutes": "Integer",
  "refreshTokenLifetimeInDays": "Integer",
  "rollingRefreshTokenLifetimeInDays": "Integer"
}
```

