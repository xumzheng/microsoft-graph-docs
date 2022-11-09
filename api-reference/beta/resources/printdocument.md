---
title: printDocument resource type
description: Represents a document being printed.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
---

# printDocument resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents a document being printed.

## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Create upload session](../api/printdocument-createuploadsession.md) | [uploadSession](uploadsession.md) | Create an upload session to iteratively upload ranges of binary file of the **printDocument**. |
| [Download binary file](../api/printdocument-get-file.md) | Download Url | Download the binary file associated with the **printDocument**. |

## Properties
| Property     | Type        | Description |
|:-------------|:------------|:------------|
|id|String|The document's identifier. Read-only.|
|displayName|String|The document's name. Read-only.|
|contentType|String|The document's content (MIME) type. Read-only.|
|size|Int64|The document's size in bytes. Read-only.|
|uploadedDateTime|Edm.DateTimeOffset|The DateTimeOffset when the document was uploaded by a client to Universal Print Server.|
|downloadedDateTime|Edm.DateTimeOffset|The DateTimeOffset when the document was downloaded by a printer from Universal Print Server.|

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printDocument"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "contentType": "String",
  "size": 12345
}

```


