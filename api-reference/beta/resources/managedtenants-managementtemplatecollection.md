---
title: "managementTemplateCollection resource type"
description: "Represent a collection of management templates that are used to define the group of actions and settings for a managed tenant."
author: "idwilliams"
ms.localizationpriority: medium
ms.prod: "microsoft-365-lighthouse"
doc_type: resourcePageType
---

# managementTemplateCollection resource type

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represent a collection of [microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md) resources used to define the group of actions and settings for a [microsoft.graph.managedTenants.managedTenant](../resources/managedtenants-managedtenant.md).

## Methods

|Method|Return type|Description|
|:---|:---|:---|
|[List managementTemplateCollections](../api/managedtenants-managedtenant-list-managementtemplatecollections.md)|[microsoft.graph.managedTenants.managementTemplateCollection](../resources/managedtenants-managementtemplatecollection.md) collection|Get a list of the [managementTemplateCollection](../resources/managedtenants-managementtemplatecollection.md) objects and their properties.|
|[Get managementTemplateCollection](../api/managedtenants-managementtemplatecollection-get.md)|[microsoft.graph.managedTenants.managementTemplateCollection](../resources/managedtenants-managementtemplatecollection.md)|Read the properties and relationships of a [managementTemplateCollection](../resources/managedtenants-managementtemplatecollection.md) object.|
|[List managementTemplates](../api/managedtenants-managementtemplatecollection-list-managementtemplates.md)|[microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md) collection|Get the managementTemplate resources from the managementTemplates navigation property.|

## Properties

|Property|Type|Description|
|:---|:---|:---|
|description|String|The description for the management template connection. Optional. Read-only.|
|displayName|String|The display name for the management template collection. Required. Read-only.|
|id|String|The unique identifier for the management template collection. Required. Read-only.|

## Relationships

|Relationship|Type|Description|
|:---|:---|:---|
|managementTemplates|[microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md) collection|A collection of management templates that can be used to configure Microsoft 365 services.|

## JSON representation

The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managementTemplateCollection",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementTemplateCollection",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```
