---
title: "supportedClaimConfiguration resource type"
description: "The options that the developer should use to configure the application's claim configurations"
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: "applications"
author: "alamaral"
---

# supportedClaimConfiguration resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

The options that the developer should use to configure the application's claim configurations.

## Properties

| Property | Type | Description |
|:---------------|:--------|:----------|
|nameIdPolicyFormat|String| The format in which the service provider expects the `NameID` to be sent in a SAML response. Developers configure this in Azure AD by using the [Azure Portal](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-saml-claims-customization#nameid-format).|


## JSON representation
Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.supportedClaimConfiguration"
}-->

```json
{
  "nameIdPolicyFormat": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "supportedClaimConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


