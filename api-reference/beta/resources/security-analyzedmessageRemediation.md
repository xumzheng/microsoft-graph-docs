---
title: "AnalyzedMessageRemediation resource type"
description: "This includes the information about the microsoft.security.analyzedMessageRemediation entity type"
author: "smkjain8"
ms.localizationpriority: medium
ms.prod: "security"
doc_type: resourcePageType
---

# AnalyzedMessageRemediation EntityType

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

AnalyzedMessageRemediation is an entityType defined in microsoft.graph.security namespace. This defines the configuration that needs to be sent to our action API to perform remediation action.

## Properties

|Property|Type|Description|
|:---|:---|:---|
|id|Edm.String|This is the unique identifier that is returned by the API to track the status the of the remediation action.|
|remediationName|Edm.String|The name of the remediation user wants to create.|
|severity|[microsoft.graph.security.severity](../resources/security-analyzedmessageremediation-severity.md)|The severity of remediation user wants to create. It can be low, medium and high.|
|remediationAction|[microsoft.graph.security.remediationAction](../resources/security-analyzedmessageremediation-remediationAction.md)|The admin action user wants to create.|
|description|Edm.String|The description user wants to have while creating remediation.|
|analyzedMessages|Collection([microsoft.graph.security.analyzedMessage](../resources/security-analyzedmessage.md))|The list of emails user wants to delete.|

## CSDL representation

The following is a CSDL representation of the entity.

```xml
<EntityType Name="analyzedMessageRemediation" ags:IsOwner="true">
    <Key>
        <PropertyRef Name="id" />
    </Key>
    <Property Name="id" Type="Edm.String" Nullable="false" />
    <Property Name="remediationName" Type="Edm.String" Nullable="false">
        <Annotation Term="Org.OData.Core.V1.Description" String="Name of the remediation request being created." />
    </Property>
    <Property Name="severity" Type="microsoft.graph.security.severity">
        <Annotation Term="Org.OData.Core.V1.Description" String="Severity of the remediation being created." />
    </Property>
    <Property Name="description" Type="Edm.String">
        <Annotation Term="Org.OData.Core.V1.Description" String="Free text description." />
    </Property>
    <Property Name="remediationAction" Type="microsoft.graph.security.remediationAction">
        <Annotation Term="Org.OData.Core.V1.Description" String="Type of the remediation which is equivalent to performing an action." />
    </Property>
    <NavigationProperty Name="analyzedMessages" Type="Collection(microsoft.graph.security.analyzedMessage)">
        <Annotation Term="Org.OData.Core.V1.Description" String="Collection of analyzed messages." />
    </NavigationProperty>
    <Annotation Term="Org.OData.Core.V1.Description" String="Analyzed message remediation resource in this context indicates an action performed on analyzed messages." />
</EntityType>
```
