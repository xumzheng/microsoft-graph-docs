---
title: "userFlowPageLayout resource type"
description: "Contains details about a userflow's page layout."
author: "almars"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: resourcePageType
---

# userFlowPageLayout resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contains details about a userflow's page layout.

Azure Active Directory B2C (Azure AD B2C) periodically releases improvements and fixes with each new page layout version. Organizations can browse available Azure AD B2C user flow page layouts and update them to the latest versions.

> [!IMPORTANT]
> We highly recommend you keep your page layout versions up-to-date so that all page elements reflect the latest security enhancements, accessibility standards, and your feedback.

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List pageLayouts](../api/b2cidentityuserflow-list-pagelayouts.md)|[UserFlowPageLayout](../resources/userflowpagelayout.md) collection|Get a list of the [UserFlowPageLayout](../resources/userflowpagelayout.md) objects and their properties.|
|[Get b2cIdentityUserFlowPageLayout](../api/b2cidentityuserflow-get-pagelayouts.md)|[UserFlowPageLayout](../resources/b2cidentityuserflow-userflowpagelayout.md)|Read the properties and relationships of a [UserFlowPageLayout](../resources/userflowpagelayout.md) object.|
|[Update userFlowPageLayout](../api/b2cidentityuserflow-update-pagelayouts)|[userFlowPageLayout](../resources/userflowpagelayout.md)|Update the properties of a [userFlowPageLayout](../resources/userflowpagelayout.md) object.|
|[availableVersions](../api/b2cidentityuserflow-pagelayout-availableversions.md)|String collection|Show the supported version of page layout to provide admins and developers the exact values allowed to use.|
|[restoreDefaultPageUri](../api/b2cidentityuserflow-pagelayout-restoredefaultpageuri.md)|None|Restore the default value of the "pageUri" property.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|Page name used to provide more description. Read-only.|
|id|String|ID of the page layout, as used in the service. Read-only.|
|isCustomPageUri|Boolean|If the page has a custom page uri, for query purpose. Read-only.|
|pageUri|String|Location for the ".html" resource used to load the custom content, as show in [documentation](https://docs.microsoft.com/azure/active-directory-b2c/customize-ui-with-html?pivots=b2c-user-flow#4-update-the-user-flow).|
|version|String|Version of the page layout.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userFlowPageLayout",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userFlowPageLayout",
  "id": "String (identifier)",
  "displayName": "String",
  "isCustomPageUri": "Boolean",
  "pageUri": "String",
  "version": "String"
}
```

