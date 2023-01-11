---
title: "recommendation resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
doc_type: resourcePageType
---

# recommendation resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [recommendationBase](../resources/recommendationbase.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List recommendations](../api/directory-list-recommendations.md)|[recommendation](../resources/recommendation.md) collection|Get a list of the [recommendation](../resources/recommendation.md) objects and their properties.|
|[Create recommendation](../api/directory-post-recommendations.md)|[recommendation](../resources/recommendation.md)|Create a new [recommendation](../resources/recommendation.md) object.|
|[Get recommendation](../api/recommendation-get.md)|[recommendation](../resources/recommendation.md)|Read the properties and relationships of a [recommendation](../resources/recommendation.md) object.|
|[Update recommendation](../api/recommendation-update.md)|[recommendation](../resources/recommendation.md)|Update the properties of a [recommendation](../resources/recommendation.md) object.|
|[Delete recommendation](../api/directory-delete-recommendations.md)|None|Delete a [recommendation](../resources/recommendation.md) object.|
|[postpone](../api/recommendation-postpone.md)|[recommendation](../resources/recommendation.md)|**TODO: Add Description**|
|[dismiss](../api/recommendation-dismiss.md)|[recommendation](../resources/recommendation.md)|**TODO: Add Description**|
|[complete](../api/recommendation-complete.md)|[recommendation](../resources/recommendation.md)|**TODO: Add Description**|
|[reactivate](../api/recommendation-reactivate.md)|[recommendation](../resources/recommendation.md)|**TODO: Add Description**|
|[List impactedResources](../api/recommendationbase-list-impactedresources.md)|[impactedResource](../resources/impactedresource.md) collection|Get the impactedResource resources from the impactedResources navigation property.|
|[Create impactedResource](../api/recommendation-post-impactedresources.md)|[impactedResource](../resources/impactedresource.md)|Create a new impactedResource object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|actionSteps|[actionStep](../resources/actionstep.md) collection|**TODO: Add Description** Inherited from [recommendationBase](../resources/recommendationbase.md).|
|benefits|String|**TODO: Add Description** Inherited from [recommendationBase](../resources/recommendationbase.md).|
|category|recommendationCategory|**TODO: Add Description** Inherited from [recommendationBase](../resources/recommendationbase.md).The possible values are: `identityBestPractice`, `identitySecureScore`, `unknownFutureValue`.|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [recommendationBase](../resources/recommendationbase.md).|
|currentScore|Double|**TODO: Add Description** Inherited from [recommendationBase](../resources/recommendationbase.md).|
|displayName|String|**TODO: Add Description** Inherited from [recommendationBase](../resources/recommendationbase.md).|
|featureAreas|recommendationFeatureAreas collection|**TODO: Add Description** Inherited from [recommendationBase](../resources/recommendationbase.md).|
|id|String|**TODO: Add Description** Inherited from [recommendationBase](../resources/recommendationbase.md).|
|impactStartDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [recommendationBase](../resources/recommendationbase.md).|
|impactType|String|**TODO: Add Description** Inherited from [recommendationBase](../resources/recommendationbase.md).|
|insights|String|**TODO: Add Description** Inherited from [recommendationBase](../resources/recommendationbase.md).|
|lastCheckedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [recommendationBase](../resources/recommendationbase.md).|
|lastModifiedBy|String|**TODO: Add Description** Inherited from [recommendationBase](../resources/recommendationbase.md).|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [recommendationBase](../resources/recommendationbase.md).|
|maxScore|Double|**TODO: Add Description** Inherited from [recommendationBase](../resources/recommendationbase.md).|
|postponeUntilDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [recommendationBase](../resources/recommendationbase.md).|
|priority|recommendationPriority|**TODO: Add Description** Inherited from [recommendationBase](../resources/recommendationbase.md).The possible values are: `low`, `medium`, `high`.|
|recommendationType|recommendationType|**TODO: Add Description** Inherited from [recommendationBase](../resources/recommendationbase.md).The possible values are: `adfsAppsMigration`, `enableDesktopSSO`, `enablePHS`, `enableProvisioning`, `switchFromPerUserMFA`, `tenantMFA`, `thirdPartyApps`, `turnOffPerUserMFA`, `useAuthenticatorApp`, `useMyApps`, `staleApps`, `staleAppCreds`, `applicationCredentialExpiry`, `servicePrincipalKeyExpiry`, `adminMFAV2`, `blockLegacyAuthentication`, `integratedApps`, `mfaRegistrationV2`, `pwagePolicyNew`, `passwordHashSync`, `oneAdmin`, `roleOverlap`, `selfServicePasswordReset`, `signinRiskPolicy`, `userRiskPolicy`, `verifyAppPublisher`, `privateLinkForAAD`, `appRoleAssignmentsGroups`, `appRoleAssignmentsUsers`, `managedIdentity`, `overprivilegedApps`, `unknownFutureValue`.|
|remediationImpact|String|**TODO: Add Description** Inherited from [recommendationBase](../resources/recommendationbase.md).|
|status|recommendationStatus|**TODO: Add Description** Inherited from [recommendationBase](../resources/recommendationbase.md).The possible values are: `active`, `completedBySystem`, `completedByUser`, `dismissed`, `postponed`, `unknownFutureValue`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|impactedResources|[impactedResource](../resources/impactedresource.md) collection|**TODO: Add Description** Inherited from [Microsoft.AAD.Reporting.recommendationBase](../resources/recommendationbase.md)|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.recommendation",
  "baseType": "Microsoft.AAD.Reporting.recommendationBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.recommendation",
  "id": "String (identifier)",
  "actionSteps": [
    {
      "@odata.type": "microsoft.graph.actionStep"
    }
  ],
  "benefits": "String",
  "category": "String",
  "createdDateTime": "String (timestamp)",
  "currentScore": "Double",
  "displayName": "String",
  "featureAreas": [
    "String"
  ],
  "impactType": "String",
  "impactStartDateTime": "String (timestamp)",
  "insights": "String",
  "lastCheckedDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": "String",
  "maxScore": "Double",
  "postponeUntilDateTime": "String (timestamp)",
  "priority": "String",
  "status": "String",
  "remediationImpact": "String",
  "recommendationType": "String"
}
```

