---
title: "recommendation resource type"
description: "Represents an Azure AD best practice or improvement action recommended by Microsoft for your Azure AD tenant."
author: "hafowler"
ms.localizationpriority: medium
ms.prod: "identity-and-access"
doc_type: resourcePageType
---

# recommendation resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents an Azure AD best practice or improvement action recommended by Microsoft for your Azure AD tenant.

The Azure AD recommendation service runs daily to check your tenant against predefined conditions for every recommendation. If the service detects that a recommendation applies to your tenant, the corresponding recommendation object is generated and its status is set to active.

There supported recommendations include the following:

1. Convert from per user MFA to Conditional Access MFA
2. Minimize MFA prompts for users signing in from known devices
3. Migrate apps from AD FS to Azure AD
4. Migrate eligible users from SMS and voice call to use the Authenticator app

For more information, see [What is Azure Active Directory recommendations?](https://go.microsoft.com/fwlink/?linkid=2221712).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List recommendations](../api/recommendation-list.md)|[recommendation](../resources/recommendation.md) collection|Get a list of the [recommendation](../resources/recommendation.md) objects and their properties.|
|[Get recommendation](../api/recommendation-get.md)|[recommendation](../resources/recommendation.md)|Read the properties and relationships of a [recommendation](../resources/recommendation.md) object.|
|[Postpone](../api/recommendation-postpone.md)|[recommendation](../resources/recommendation.md)|Mark the status of a [recommendation](../resources/recommendation.md) object as `postponed` to a specified date and time.|
|[Dismiss](../api/recommendation-dismiss.md)|[recommendation](../resources/recommendation.md)|Mark the status of a [recommendation](../resources/recommendation.md) object as `dismissed`.|
|[Complete](../api/recommendation-complete.md)|[recommendation](../resources/recommendation.md)|Mark the status of a [recommendation](../resources/recommendation.md) object as `completedByUser`.|
|[Reactivate](../api/recommendation-reactivate.md)|[recommendation](../resources/recommendation.md)|Mark the status of a [recommendation](../resources/recommendation.md) object as `active`.|
|[List impactedResources](../api/recommendation-list-impactedresources.md)|[impactedResource](../resources/impactedresource.md) collection|Get the [impactedResource](../resources/impactedresource.md) resources from the impactedResources navigation property.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|actionSteps|[actionStep](../resources/actionstep.md) collection|List of actions to take to complete a [recommendation](../resources/recommendation.md)|
|benefits|String|An explanation of why [completing the recommendation](../api/recommendation-complete.md) will benefit you. Corresponds to the *Value* section of a recommendation shown in the Azure AD portal.|
|category|recommendationCategory|Indicates the category of intelligent guidance the recommendation falls under. The possible values are: `identityBestPractice`, `identitySecureScore`, `unknownFutureValue`.|
|createdDateTime|DateTimeOffset|The date and time when the [recommendation](../resources/recommendation.md) was detected as applicable to your directory.|
|currentScore|Double|The number of points the tenant has attained. Only applies to [recommendations](../resources/recommendation.md) with **category** set to `identitySecureScore`.|
|displayName|String|The title of the [recommendation](../resources/recommendation.md).|
|featureAreas|recommendationFeatureAreas collection|The directory feature that the [recommendation](../resources/recommendation.md) is related to.|
|id|String|The unique identifier for the [recommendation](../resources/recommendation.md) object generated for your tenant.|
|impactStartDateTime|DateTimeOffset|The future date and time when a [recommendation](../resources/recommendation.md) should be completed.|
|impactType|String|	Indicates the scope of impact of a recommendation. `Tenant level` indicates that the recommendation impacts the whole tenant. Other possible values include `users`, `applications`.|
|insights|String|Describes why a recommendation uniquely applies to your directory. Corresponds to the *Description* section of a recommendation shown in the Azure AD portal.|
|lastCheckedDateTime|DateTimeOffset|The most recent date and time a [recommendation](../resources/recommendation.md) was deemed applicable to your directory.|
|lastModifiedBy|String|Name of the user who last updated the **status** of the [recommendation](../resources/recommendation.md).|
|lastModifiedDateTime|DateTimeOffset|	The date and time the **status** of a [recommendation](../resources/recommendation.md) was last updated.|
|maxScore|Double|The maximum number of points attainable. Only applies to [recommendations](../resources/recommendation.md) with **category** set to `identitySecureScore`.|
|postponeUntilDateTime|DateTimeOffset|The future date and time when the **status** of a postponed [recommendation](../resources/recommendation.md) will be `active` again.|
|priority|recommendationPriority|Indicates the time sensitivity for a [recommendation](../resources/recommendation.md) to be completed. Microsoft auto assigns this value. The possible values are: `low`, `medium`, `high`. Read-only.|
|recommendationType|recommendationType|Friendly shortname to identify the [recommendation](../resources/recommendation.md). The possible values are: `adfsAppsMigration`, `enableDesktopSSO`, `enablePHS`, `enableProvisioning`, `switchFromPerUserMFA`, `tenantMFA`, `thirdPartyApps`, `turnOffPerUserMFA`, `useAuthenticatorApp`, `useMyApps`, `staleApps`, `staleAppCreds`, `applicationCredentialExpiry`, `servicePrincipalKeyExpiry`, `adminMFAV2`, `blockLegacyAuthentication`, `integratedApps`, `mfaRegistrationV2`, `pwagePolicyNew`, `passwordHashSync`, `oneAdmin`, `roleOverlap`, `selfServicePasswordReset`, `signinRiskPolicy`, `userRiskPolicy`, `verifyAppPublisher`, `privateLinkForAAD`, `appRoleAssignmentsGroups`, `appRoleAssignmentsUsers`, `managedIdentity`, `overprivilegedApps`, `unknownFutureValue`.|
|remediationImpact|String|Description of the impact on users of the remediation. Only applies to [recommendations](../resources/recommendation.md) with **category** set to `identitySecureScore`.|
|status|recommendationStatus|	Indicates the status of the [recommendation](../resources/recommendation.md) based on user or system action. The possible values are: `active`, `completedBySystem`, `completedByUser`, `dismissed`, `postponed`, `unknownFutureValue`. By default, a recommendation's **status** is set to `active` when the recommendation is first generated. **Status** is set to `completedBySystem` when our service detects that a recommendation which was previously active no longer applies.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|impactedResources|[impactedResource](../resources/impactedresource.md) collection|The list of directory objects associated with the [recommendation](../resources/recommendation.md).|

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

