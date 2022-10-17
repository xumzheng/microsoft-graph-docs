---
title: "threatSubmissionRoot resource type"
description: "Represents threat submission root"
author: "caigen"
ms.localizationpriority: medium
ms.prod: "security"
doc_type: resourcePageType
---

# threatSubmissionRoot resource type

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Threat submission root is a unified threat submission node under `security`. It is singleton instance without methods and provides the unified threat submission API surface to customers. 

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|The Id. Inherited from [entity](../resources/entity.md).|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
| emailThreats | [microsoft.graph.security.emailThreatSubmission](../resources/security-emailthreatsubmission.md) collection. | Reports suspected spam, malware or phishing emails to Microsoft Defender for Office 365. |
| emailThreatSubmissionPolicies | [microsoft.graph.security.emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md) collection. | Represents the guidelines of an organization to report potential threats and spam messages. |
| fileThreats | [microsoft.graph.security.fileThreatSubmission](../resources/security-filethreatsubmission.md) collection. | Represents threat submissions related to a file. |
| urlThreats | [microsoft.graph.security.urlThreatSubmission](../resources/security-urlthreatsubmission.md) collection. | Represent a threat submission related to a URL. |

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.threatSubmissionRoot",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.threatSubmissionRoot",
  "id": "String (identifier)"
}
```

