---
title: "ipApplicationSegment resource type"
description: "Represents the segment configurations that are allowed for an on-premises non web application published through Azure AD Application Proxy."
ms.localizationpriority: medium
author: "katabish"
ms.prod: "applications"
doc_type: "resourcePageType"
---

# ipApplicationSegment resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

An [ipApplicationSegment](ipapplicationsegment.md) object represents the segment configurations that are allowed for an on-premises non web application published through Azure AD Application Proxy.

Inherits from [applicationSegment](applicationsegment.md).

## Properties

| Property     | Type        | Description |
|:-------------|:------------|:------------|
|destinationHost| String | IP address, IP range, or FQDN of the applicationSegment.|
|id|String|The unique identifier that is assigned to an applicationSegment by Azure AD. Not nullable. Read-only. Supports `$filter` (`eq`). Inherited from [applicationSegment](applicationsegment.md).|
|port (Deprecated)| String | Port supported for the application segment.|
|ports| [String] | List of ports supported for the application segment.|

## JSON representation

The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.webApplicationSegment"
}
-->
``` json
{
  "@odata.type": "microsoft.graph.ipApplicationSegment",
  "destinationHost": "String",
  "port": "String",
  "ports": ["String"]
}
```