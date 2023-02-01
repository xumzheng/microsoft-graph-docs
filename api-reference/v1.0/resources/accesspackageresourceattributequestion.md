---
title: "accessPackageResourceAttributeQuestion resource type"
description: "Resource that defines the question provided to an end user, for the purpose of obtaining an attribute value to be passed to the end system or the request approver."
author: "saylee-dharne-msft"
ms.localizationpriority: medium
ms.prod: "governance"
doc_type: resourcePageType
---

# accessPackageResourceAttributeQuestion resource type

Namespace: microsoft.graph



Resource that defines the [question](accesspackagequestion.md) provided to an end user, for the purpose of obtaining an attribute value to be passed to the end system or the request approver.

This type inherits from [accessPackageResourceAttributeSource](../resources/accesspackageresourceattributesource.md) and is used in the **attributeSource** property of an [accessPackageResourceAttribute](accesspackageresourceattribute.md).

Inherits from [accessPackageResourceAttributeSource](../resources/accesspackageresourceattributesource.md).

## Properties
None.

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|question|[accessPackageQuestion](../resources/accesspackagequestion.md)|The question asked in order to get the value of the attribute. |

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageResourceAttributeQuestion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageResourceAttributeQuestion"
}
```

