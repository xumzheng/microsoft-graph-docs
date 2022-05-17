---
title: "managementTemplateStepDeployment resource type"
description: "Represents the deployment detail for a management template used to configure Microsoft 365 services."
author: "idwilliams"
ms.localizationpriority: medium
ms.prod: "microsoft-365-lighthouse"
doc_type: resourcePageType
---

# managementTemplateStepDeployment resource type

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents the deployment detail for a management template used to configure Microsoft 365 services.

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List managementTemplateStepDeployments](../api/managedtenants-managementtemplatestepdeployment-list.md)|[microsoft.graph.managedTenants.managementTemplateStepDeployment](../resources/managedtenants-managementtemplatestepdeployment.md) collection|Get a list of the [managementTemplateStepDeployment](../resources/managedtenants-managementtemplatestepdeployment.md) objects and their properties.|
|[Get managementTemplateStepDeployment](../api/managedtenants-managementtemplatestepdeployment-get.md)|[microsoft.graph.managedTenants.managementTemplateStepDeployment](../resources/managedtenants-managementtemplatestepdeployment.md)|Read the properties and relationships of a [managementTemplateStepDeployment](../resources/managedtenants-managementtemplatestepdeployment.md) object.|
|[changeDeploymentStatus](../api/managedtenants-managementtemplatestepdeployment-changedeploymentstatus.md)|[microsoft.graph.managedTenants.managementTemplateStepDeployment](../resources/managedtenants-managementtemplatestepdeployment.md)|Changes the status for the given management template step deployment.|
|[List templateStepVersion](../api/managedtenants-managementtemplatestepdeployment-list-templatestepversion.md)|[microsoft.graph.managedTenants.managementTemplateStepVersion](../resources/managedtenants-managementtemplatestepversion.md) collection|Get the managementTemplateStepVersion resources from the templateStepVersion navigation property.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|error|[microsoft.graph.managedTenants.graphAPIErrorDetails](../resources/managedtenants-graphapierrordetails.md)|The error details if one was encountered during deployment of the management step. Required. Read-only.|
|id|String|The unique identifier for the management template step deployment. Required. Read-only.|
|settings|[microsoft.graph.managedTenants.setting](../resources/managedtenants-setting.md) collection|The collection of settings used by the management step deployment. Optional. Read-only.|
|status|[microsoft.graph.managedTenants.managementTemplateDeploymentStatus](#managementtemplatedeploymentstatus-values)|The status for the management template step deployment..The possible values are: `toAddress`, `completed`, `error`, `timeOut`, `inProgress`, `planned`, `resolvedBy3rdParty`, `resolvedThroughAlternateMitigation`, `riskAccepted`, `unknownFutureValue`. Required.|
|tenantId|String|The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md). Required. Read-only.|

### managementTemplateDeploymentStatus values

|Member|Description|
|:---|:---|
|toAddress|Represents the deployment has not been addressed.|
|completed|Represents the management template deployment has been completed.|
|error|Represents the management template deployment encountered an error when it was deployed.|
|timeOut|Represents the request to deploy the management template timed out when attempting to deploy.|
|inProgress|Represents the management template deployment is currently in progress.|
|planned|Represents the management template deployment has been planned.|
|resolvedBy3rdParty|Represent the intent of the management template deployment has been fulfilled by a third party.|
|resolvedThroughAlternateMitigation|Represents the intent of the management template step has been fulfilled by alternate mitigation.|
|riskAccepted|Represents the intent of the management template deployment is an accepted risk.|
|unknownFutureValue|Represents a future or unknown value.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|templateStepVersion|[microsoft.graph.managedTenants.managementTemplateStepVersion](../resources/managedtenants-managementtemplatestepversion.md)|The version for the management template step.|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managementTemplateStepDeployment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementTemplateStepDeployment",
  "id": "String (identifier)",
  "tenantId": "String",
  "settings": [
    {
      "@odata.type": "microsoft.graph.managedTenants.setting"
    }
  ],
  "status": "String",
  "error": {
    "@odata.type": "microsoft.graph.managedTenants.graphAPIErrorDetails"
  }
}
```
