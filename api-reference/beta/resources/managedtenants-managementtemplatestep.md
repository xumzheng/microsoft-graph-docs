---
title: "managementTemplateStep resource type"
description: "Represents the settings that can be used to configure Microsoft 365 services."
author: "idwilliams"
ms.localizationpriority: medium
ms.prod: "microsoft-365-lighthouse"
doc_type: resourcePageType
---

# managementTemplateStep resource type

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents the settings that can be used to configure Microsoft 365 services.

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List managementTemplateSteps](../api/managedtenants-managedtenant-list-managementtemplatesteps.md)|[microsoft.graph.managedTenants.managementTemplateStep](../resources/managedtenants-managementtemplatestep.md) collection|Get a list of the [microsoft.graph.managedTenants.managementTemplateStep](../resources/managedtenants-managementtemplatestep.md) objects and their properties.|
|[Get managementTemplateStep](../api/managedtenants-managementtemplatestep-get.md)|[microsoft.graph.managedTenants.managementTemplateStep](../resources/managedtenants-managementtemplatestep.md)|Read the properties and relationships of a [microsoft.graph.managedTenants.managementTemplateStep](../resources/managedtenants-managementtemplatestep.md) object.|
|[List managementTemplate](../api/managedtenants-managementtemplatestep-list-managementtemplate.md)|[microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md) collection|Get the **managementTemplate** resources associated with the **managementTemplateStep**.|
|[List stepVersions](../api/managedtenants-managementtemplatestep-list-stepversions.md)|[microsoft.graph.managedTenants.managementTemplateStepVersion](../resources/managedtenants-managementtemplatestepversion.md) collection|Get the **managementTemplateStepVersion** resources associated with the **managementTemplateStep**.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|category|managementCategory|The category for the management template. The possible values are: `custom`, `devices`, `identity`, `data`, `unknownFutureValue`. Required. Read-only.|
|description|String|The description for the management template step. Optional. Read-only.|
|displayName|String|The display name for the management template step. Optional. Read-only.|
|id|String|The unique identifier for the management template step. Required. Read-only.|
|managementPortal|String|The display name for the management portal of the workload (e.g., Azure Active Directory, Microsoft Endpoint Manager) where service specific management actions can be performed. Required.|
|portalLink|String|The link for the management where further actions can be taken. Required.|
|priority|Int32|The position in the sequence where the management template should be applied. Required.|
|provider|[microsoft.graph.managedTenants.managementProvider](#managementprovider-values)|The provider for the management template step. The possible values are: `microsoft`, `community`, `indirectProvider`, `self`, `unknownFutureValue`. Required. Read-only.|

### managementProvider values

|Member|Description|
|:---|:---|
|microsoft|Indicates that Microsoft is the provider.|
|community|Indicates the community is the provider.|
|indirectProvider|Indicates that an indirect provider is the provider.|
|self|Indicates the managing entity is the provider.|
|unknownFutureValue|Evolvable enumeration sentinel value. Do not use|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|managementTemplate|[microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md)|The management template associated with the management template step.|
|stepVersions|[microsoft.graph.managedTenants.managementTemplateStepVersion](../resources/managedtenants-managementtemplatestepversion.md) collection|The collection of management template step versions.|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managementTemplateStep",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementTemplateStep",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": "Integer",
  "category": "String",
  "provider": "String",
  "managementPortal": "String",
  "portalLink": "String"
}
```
