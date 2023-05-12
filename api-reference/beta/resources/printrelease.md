---
title: "printRelease complex type"
description: "Represents the job release options supported by a printer."
author: "venkatnagula"
ms.localizationpriority: medium
ms.prod: "cloud-printing"
doc_type: resourcePageType
---

# printRelease complex type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents the job release options supported by a printer.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|releaseType|printReleaseType|Supported print release type|

## printReleaseType values

|Member|Value|Description|
|:---|:---|:---|
|direct|0|Print job is released to printer immediately after the print job is processed by Universal Print.|
|qrCode|1|Print job is held within Universal Print until user scans the QR code and completes the release workflow.|
|unknownFutureValue|2|Evolvable enumeration sentinel value. Do not use.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printRelease"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printRelease",
  "releaseType": {"@odata.type": "microsoft.graph.printReleaseType"}
}
```
