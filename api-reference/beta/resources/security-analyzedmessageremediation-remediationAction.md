---
title: "RemediationAction enum type"
description: "This includes the information about the microsoft.security.remediationAction enum type"
author: "smkjain8"
ms.localizationpriority: medium
ms.prod: "security"
doc_type: resourcePageType
---

# RemediationAction EnumType

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

RemediationAction enum defines the type of remediation action that the user wants to perform on single or bunch of emails received in the tenant.

## Members

|Name|Value|Description|
|:---|:---|:---|
|softDelete|1|Soft Delete analyzed messages.|
|hardDelete|2|Hard Delete analyzed messages.|
|moveToJunk|3|Move analyzed messages to junk folder.|
|moveToInbox|4|Move analyzed messages to inbox folder.|
|unknownFutureValue|5|New action not defined yet.|

## CSDL representation

The following is a CSDL representation of the enum.

```xml
<EnumType Name="remediationAction">
    <Member Name="softDelete" Value="1">
        <Annotation Term="Org.OData.Core.V1.Description" String="Soft Delete analyzed messages." />
    </Member>
    <Member Name="hardDelete" Value="2">
        <Annotation Term="Org.OData.Core.V1.Description" String="Hard Delete analyzed messages." />
    </Member>
    <Member Name="moveToJunk" Value="3">
        <Annotation Term="Org.OData.Core.V1.Description" String="Move analyzed messages to junk folder." />
    </Member>
    <Member Name="moveToInbox" Value="4">
        <Annotation Term="Org.OData.Core.V1.Description" String="Move analyzed messages to inbox folder." />
    </Member>
    <Member Name="unknownFutureValue" Value="5"/>
    <Annotation Term="Org.OData.Core.V1.Description" String="AnalyzedMessage Remediation types." />
</EnumType>
```
