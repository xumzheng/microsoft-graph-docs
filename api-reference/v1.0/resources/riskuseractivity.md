---
title: "riskUserActivity resource type"
description: "Represents the risk activities of an Azure Active Directory (Azure AD) user as determined by Azure AD Identity Protection."
author: "tracyshi"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: resourcePageType
---

# riskUserActivity resource type

Namespace: microsoft.graph

Represents the risk activities of an Azure Active Directory (Azure AD) user as determined by Azure AD Identity Protection.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|detail|riskDetail|Details of the detected risk. Supports a subset of the values for **riskDetail**. Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`, `m365DAdminDismissedDetection`. Note that you must use the `Prefer: include-unknown-enum-members` request header to get the following values in this [evolvable enum](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `m365DAdminDismissedDetection`.|
|riskEventTypes|String collection|The type of risk event detected.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.riskUserActivity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.riskUserActivity",
  "detail": "String",
  "riskEventTypes": [
    "String"
  ]
}
```
