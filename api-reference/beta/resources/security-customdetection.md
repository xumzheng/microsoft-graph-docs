---
title: "customDetection resource type"
description: "Represents custom detection rules over hunting queries that run by schedule and trigger alerts on any matching result"
author: "mmekler"
ms.localizationpriority: medium
ms.prod: "security"
doc_type: resourcePageType
---

# customDetection resource type

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Custom detection rules are rules you can design and tweak using advanced hunting queries. These rules let you proactively monitor various events and system states, including suspected breach activity and misconfigured endpoints.
You can set them to run at regular intervals, generating alerts and taking response actions whenever there are matches.


Inherits from [microsoft.graph.entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List customDetections](../api/security-security-list-customdetections.md)|[microsoft.graph.security.customDetection](../resources/security-customdetection.md) collection|Get a list of the [microsoft.graph.security.customDetection](../resources/security-customdetection.md) objects and their properties.|
|[Create customDetection](../api/security-post-customdetections.md)|[microsoft.graph.security.customDetection](../resources/security-customdetection.md)|Create a new [microsoft.graph.security.customDetection](../resources/security-customdetection.md) object.|
|[Get customDetection](../api/security-customdetection-get.md)|[microsoft.graph.security.customDetection](../resources/security-customdetection.md)|Read the properties and relationships of a [microsoft.graph.security.customDetection](../resources/security-customdetection.md) object.|
|[Update customDetection](../api/security-customdetection-update.md)|[microsoft.graph.security.customDetection](../resources/security-customdetection.md)|Update the properties of a [microsoft.graph.security.customDetection](../resources/security-customdetection.md) object.|
|[Delete customDetection](../api/security-security-delete-customdetections.md)|None|Delete a [microsoft.graph.security.customDetection](../resources/security-customdetection.md) object.|

## Properties
| Property                | Type                                                                                                                        | Description                                                                                                                                                                                                                                                                                          |
|:------------------------|:----------------------------------------------------------------------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| actions                 | [microsoft.graph.security.customDetectionAction](../resources/security-customdetectionaction.md) collection                 | Actions taken on impacted entities as set in the custom detection rule.                                                                                                                                                                                                                              |
| alertCategory           | String                                                                                                                      | Category assigned to the alert triggered by the custom detection rule.                                                                                                                                                                                                                               |
| alertDescription        | String                                                                                                                      | Description of the alert triggered by the custom detection rule.                                                                                                                                                                                                                                     |
| alertRecommendedAction  | String                                                                                                                      | Recommended actions to mitigate the threat related to the alert triggered by the custom detection rule.                                                                                                                                                                                              |
| alertSeverity           | alertSeverity                                                                                                               | Severity assigned to the alert triggered by the custom detection rule. The possible values are: `unknown`, `informational`, `low`, `medium`, `high`, `unknownFutureValue`.                                                                                                                           |
| alertTitle              | String                                                                                                                      | Name of the alert triggered by the custom detection rule.                                                                                                                                                                                                                                            |
| createdBy               | String                                                                                                                      | Name of user who created the custom detection rule.                                                                                                                                                                                                                                                  |
| creationDateTime        | DateTimeOffset                                                                                                              | Timestamp of custom detection rule creation.                                                                                                                                                                                                                                                         |
| frequency               | String                                                                                                                      | How often the detection rule is set to run.                                                                                                                                                                                                                                                          |
| id                      | String                                                                                                                      | Unique identifier to represent the custom detection.                                                                                                                                                                                                                                                 |
| impactedEntities        | [microsoft.graph.security.customDetectionImpactedEntity](../resources/security-customdetectionimpactedentity.md) collection | Which entity or entities were impacted based on the alert triggered by the custom detection rule.                                                                                                                                                                                                    |
| isEnabled               | Boolean                                                                                                                     | Indicates whether custom detection is turned on for the tenant.                                                                                                                                                                                                                                      |
| lastQueryUpdateDateTime | DateTimeOffset                                                                                                              | Timestamp of when the query in the custom detection rule was last updated.                                                                                                                                                                                                                           |
| lastRunDateTime         | DateTimeOffset                                                                                                              | Timestamp when the custom detection was last run.                                                                                                                                                                                                                                                    |
| lastRunErrorCode        | huntingRuleErrorCode                                                                                                        | Error code of the most recent run that encountered an error. The possible values are: `queryExecutionFailed`, `queryExecutionThrottling`, `queryExceededResultSize`, `queryLimitsExceeded`, `queryTimeout`, `alertCreationFailed`, `alertReportNotFound`, `partialRowsFailed`, `unknownFutureValue`. |
| lastRunFailureReason    | String                                                                                                                      | Reason for failure when the custom detection last run and failed.                                                                                                                                                                                                                                    |
| lastRunStatus           | huntingRuleRunStatus                                                                                                        | Status of custom detection when it was last run. The possible values are: `running`, `completed`, `failed`, `partiallyFailed`, `unknownFutureValue`.                                                                                                                                                 |
| lastUpdatedBy           | String                                                                                                                      | Name of user who last updated the custom detection rule.                                                                                                                                                                                                                                             |
| lastUpdatedDateTime     | DateTimeOffset                                                                                                              | Timestamp of when the custom detection rule was last updated.                                                                                                                                                                                                                                        |
| mitreTechniques         | String collection                                                                                                           | MITRE technique assigned to the alert triggered by the custom detection rule.                                                                                                                                                                                                                        |
| nextRunDateTime         | DateTimeOffset                                                                                                              | Timestamp of the custom detection rule's next scheduled run.                                                                                                                                                                                                                                         |
| organizationalScope     | String collection                                                                                                           | List of device groups to which the custom detection rule applies.                                                                                                                                                                                                                                    |
| queryText               | String                                                                                                                      | Contents of the query.                                                                                                                                                                                                                                                                               |
| ruleName                | String                                                                                                                      | Name of the custom detection rule.                                                                                                                                                                                                                                                                   |
| serviceSources          | serviceSource collection                                                                                                    | Product or service that provided the alert information.                                                                                                                                                                                                                                              |

### alertSeverity values

| Member             | Description                                                                                                                                                                                                                                                                                                                                                                                                                   |
|:-------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| unknown		          | Unknown severity.                                                                                                                                                                                                                                                                                                                                                                                                             |
| informational	     | Alerts that may not be actionable or considered harmful to the network but can drive organizational security awareness on potential security issues.                                                                                                                                                                                                                                                                          |
| low                | Alerts on threats associated with prevalent malware. For example, hack-tools, non-malware hack tools, such as running exploration commands and clearing logs, that often don't indicate an advanced threat that targets the organization. It can also come from an isolated security tool that is tested by a user in your organization.                                                                                      |
| medium             | Alerts generated from detections and response post-breach behaviors that might be a part of an advanced persistent threat (APT). This includes observed behaviors typical of attack stages, anomalous registry change, execution of suspicious files, and so forth. Although some might be due to internal security testing, they are valid detections and require investigation as they may be a part of an advanced attack. |
| high               | Alerts commonly seen associated with advanced persistent threats (APT). These alerts indicate a high risk because of the severity of damage they can inflict on assets. Some examples are: credential theft tools activities, ransomware activities not associated with any group, tampering with security sensors, or any malicious activities indicative of a human adversary.                                              |
| unknownFutureValue | Evolvable enumeration sentinel value. Do not use.                                                                                                                                                                                                                                                                                                                                                                             |

### huntingRuleErrorCode values

| Member                     | Description                                                                                                                     |
|----------------------------|---------------------------------------------------------------------------------------------------------------------------------|
| `queryExecutionFailed`     | The query in this custom detection rule failed to run                                                                           |
| `queryExecutionThrottling` | The query in this custom detection rule was throttled due to large volume of requests it made                                   |
| `queryExceededResultSize`  | The query in this custom detection rule triggered results that exceeded the maximum number of results                           |
| `queryLimitsExceeded`      | The query in this custom detection rule exceeded resource consumption limits                                                    |
| `queryTimeout`             | The query in this custom detection rule timed out                                                                               |
| `alertCreationFailed`      | The query ran but alert creation failed                                                                                         |
| `alertReportNotFound`      | An event in the query results for this custom detection rule could not be matched to the given Timestamp, DeviceId, or ReportId |
| `partialRowsFailed`        | A portion of the custom detection rule's query results failed to trigger alerts                                                 |
| `queryTimeout`             | unknownFutureValue for evolvable enums pattern                                                                                  |

### huntingRuleRunStatus values

| Member               | Description                                      |
|----------------------|--------------------------------------------------|
| `running`            | The custom detection rule is running             |
| `completed`          | The custom detection rule completed successfully |
| `failed`             | The custom detection rule failed to run          |
| `partiallyFailed`    | The custom detection rule partially failed       |
| `unknownFutureValue` | unknownFutureValue for evolvable enums pattern   |

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.customDetection",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.customDetection",
  "id": "String (identifier)",
  "ruleName": "String",
  "isEnabled": "Boolean",
  "frequency": "String",
  "createdBy": "String",
  "creationDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "lastUpdatedBy": "String",
  "lastQueryUpdateDateTime": "String (timestamp)",
  "lastRunDateTime": "String (timestamp)",
  "lastRunStatus": "String",
  "lastRunFailureReason": "String",
  "lastRunErrorCode": "String",
  "nextRunDateTime": "String (timestamp)",
  "queryText": "String",
  "alertTitle": "String",
  "alertDescription": "String",
  "alertSeverity": "String",
  "alertCategory": "String",
  "mitreTechniques": [
    "String"
  ],
  "alertRecommendedAction": "String",
  "organizationalScope": [
    "String"
  ],
  "serviceSources": [
    "String"
  ],
  "impactedEntities": [
    {
      "@odata.type": "microsoft.graph.security.customDetectionImpactedEntity"
    }
  ],
  "actions": [
    {
      "@odata.type": "microsoft.graph.security.customDetectionAction"
    }
  ]
}
```

