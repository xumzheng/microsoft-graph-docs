---
title: "authenticationMethodsPolicy resource type"
description: "A complex type that defines settings to prompt users in the organization to use the most appropriate credentials among the ones registered by the user. Presently, a user has selected the default authentication method. With this implementation, this chosen credential is determined dynamically based on various factors including security, availability, and user experience. This credential will override the current method selected by the user. At present this will only apply to MFA. Going forward, in future releases, this will be applicable for all user authentications."
author: "msft-poulomi"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: resourcePageType
---

# authenticationMethodsPolicy resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[Get authenticationMethodsPolicy](../api/authenticationmethodspolicy-get.md)|[authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md)|Read the properties and relationships of an [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) object.|
|[Update authenticationMethodsPolicy](../api/authenticationmethodspolicy-update.md)|[authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md)|Update the properties of an [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) object.|
|[List authenticationMethodConfigurations](../api/authenticationmethodspolicy-list-authenticationmethodconfigurations.md)|[authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md) collection|Get the authenticationMethodConfiguration resources from the authenticationMethodConfigurations navigation property.|
|[Create authenticationMethodConfiguration](../api/authenticationmethodspolicy-post-authenticationmethodconfigurations.md)|[authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md)|Create a new authenticationMethodConfiguration object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|policyMigrationState|authenticationMethodsPolicyMigrationState|**TODO: Add Description**.The possible values are: `preMigration`, `migrationInProgress`, `migrationComplete`, `unknownFutureValue`.|
|policyVersion|String|**TODO: Add Description**|
|reconfirmationInDays|Int32|**TODO: Add Description**|
|registrationEnforcement|[registrationEnforcement](../resources/registrationenforcement.md)|**TODO: Add Description**|
|systemCredentialPreferences|[systemCredentialPreferences](../resources/systemcredentialpreferences.md)|"Credential preference for all user authentications is calculated at runtime and prompted to the user. This overrides the user-selected authentication method. Note that presently, it will be enforced only for MFA. Going forward, in future releases, this will be enforced for all authentications."|
|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|authenticationMethodConfigurations|[authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationMethodsPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodsPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "policyVersion": "String",
  "policyMigrationState": "String",
  "registrationEnforcement": {
    "@odata.type": "microsoft.graph.registrationEnforcement"
  },
  "reconfirmationInDays": "Integer",
  "systemCredentialPreferences": {
    "@odata.type": "microsoft.graph.systemCredentialPreferences"
  }
}
```

