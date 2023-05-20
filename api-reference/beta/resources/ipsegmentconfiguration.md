---
title: "ipSegmentConfiguration resource type"
description: "Represents application segments for an on-premises non web application published through Azure AD Application Proxy."
ms.localizationpriority: medium
author: "katabish"
ms.prod: "applications"
doc_type: "resourcePageType"
---

# ipSegmentConfiguration resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

An [ipSegmentConfiguration](ipsegmentconfiguration.md) object represents application segments for an on-premises non web application published through Azure AD Application Proxy.

Inherits from [segmentsConfiguration](segmentconfiguration.md).

## Properties

| Property     | Type        | Description |
|:-------------|:------------|:------------|
|applicationSegments|[ipApplicationSegment](ipapplicationsegment.md) collection|A collection of application segments for an on-premises non web application published through Azure AD Application Proxy. It includes the destinationHost and ports. |


## JSON representation

The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.onPremisesApplicationSegment"
}
-->
``` json
{
 "@odata.type": "#microsoft.graph.ipSegmentConfiguration",
 "applicationSegments": [
    {
      "@odata.type": "microsoft.graph.ipApplicationSegment"
    }
  ],
}
```