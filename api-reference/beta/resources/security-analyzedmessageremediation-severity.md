---
title: "Severity enum type"
description: "This includes the information about the microsoft.security.severity enum type"
author: "smkjain8"
ms.localizationpriority: medium
ms.prod: "security"
doc_type: resourcePageType
---

# Severity EnumType

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Severity enum defines the severity with which the admin wants to perform the remediation action.

## Members

|Name|Value|Description|
|:---|:---|:---|
|high|1|Severity is high.|
|medium|2|Severity is medium.|
|low|3|Severity is low.|
|unknownFutureValue|4|Severity is not defined yet.|

## CSDL representation

The following is a CSDL representation of the enum.

```xml
<EnumType Name="severity">
    <Member Name="high" Value="1">
        <Annotation Term="Org.OData.Core.V1.Description" String="Severity is high." />
    </Member>
    <Member Name="medium" Value="2">
        <Annotation Term="Org.OData.Core.V1.Description" String="Severity is medium." />
    </Member>
    <Member Name="low" Value="3">
        <Annotation Term="Org.OData.Core.V1.Description" String="Severity is low." />
    </Member>
    <Member Name="unknownFutureValue" Value="4"/>
    <Annotation Term="Org.OData.Core.V1.Description" String="Severity of the remediation ." />
</EnumType>
```
