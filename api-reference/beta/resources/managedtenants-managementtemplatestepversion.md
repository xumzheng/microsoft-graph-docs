---
title: "managementTemplateStepVersion resource type"
description: "Represents actions and settings used to configure Microsoft 365 services."
author: "idwilliams"
ms.localizationpriority: medium
ms.prod: "microsoft-365-lighthouse"
doc_type: resourcePageType
---

# managementTemplateStepVersion resource type

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents actions and settings used to configure Microsoft 365 services.

## Methods

|Method|Return type|Description|
|:---|:---|:---|
|[List managementTemplateStepVersions](../api/managedtenants-managedtenant-list-managementtemplatestepversions.md)|[microsoft.graph.managedTenants.managementTemplateStepVersion](../resources/managedtenants-managementtemplatestepversion.md) collection|Get a list of the [microsoft.graph.managedTenants.managementTemplateStepVersion](../resources/managedtenants-managementtemplatestepversion.md) objects and their properties.|
|[Get managementTemplateStepVersion](../api/managedtenants-managementtemplatestepversion-get.md)|[microsoft.graph.managedTenants.managementTemplateStepVersion](../resources/managedtenants-managementtemplatestepversion.md)|Read the properties and relationships of a [microsoft.graph.managedTenants.managementTemplateStepVersion](../resources/managedtenants-managementtemplatestepversion.md) object.|
|[deploy](../api/managedtenants-managementtemplatestepversion-deploy.md)|[microsoft.graph.managedTenants.managementTemplateStepDeployment](../resources/managedtenants-managementtemplatestepdeployment.md)|Deploys the actions and settings to the specific tenant configuring the Microsoft 365 services represented by the management template step version.|
|[List deployments](../api/managedtenants-managementtemplatestepversion-list-deployments.md)|[microsoft.graph.managedTenants.managementTemplateStepDeployment](../resources/managedtenants-managementtemplatestepdeployment.md) collection|Gets the [microsoft.graph.managedtenants.managementTemplateStepDeployment](../resources/managedtenants-managementtemplatestepdeployment.md) resources with a management template step version.|
|[List templateStep](../api/managedtenants-managementtemplatestepversion-list-templatestep.md)|[microsoft.graph.managedTenants.managementTemplateStep](../resources/managedtenants-managementtemplatestep.md) collection|Gets the [microsoft.graph.managedtenants-managementtemplatestep.md](../resources/managedtenants-managementtemplatestep.md) resources associated with a management template step version.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|configurationAction|[microsoft.graph.managedTenants.templateAction](../resources/managedtenants-templateaction.md)|The actions and settings used to configure a specific Microsoft 365 service. Required. Read-only.|
|id|String|The unique identifier for the management template step version. Required. Read-only.|
|validationAction|[microsoft.graph.managedTenants.templateAction](../resources/managedtenants-templateaction.md)|The manage action used to measure if the actions or configurations completed.|
|version|Int32|The version of the management template step. Required. Read-only.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|deployments|[microsoft.graph.managedTenants.managementTemplateStepDeployment](../resources/managedtenants-managementtemplatestepdeployment.md) collection|The collection of deployments associated with the management template step version.|
|templateStep|[microsoft.graph.managedTenants.managementTemplateStep](../resources/managedtenants-managementtemplatestep.md)|The details for what should be configured or performed when the management template step version is deployed.|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managementTemplateStepVersion",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementTemplateStepVersion",
  "id": "String (identifier)",
  "configurationAction": {
    "@odata.type": "microsoft.graph.managedTenants.templateAction"
  },
  "validationAction": {
    "@odata.type": "microsoft.graph.managedTenants.templateAction"
  },
  "version": "Integer"
}
```
