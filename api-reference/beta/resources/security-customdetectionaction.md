---
title: "customDetectionAction resource type"
description: "Each custom detection rule contains a list of actions to be taken on impacted entities"
author: "mmekler"
ms.localizationpriority: medium
ms.prod: "security"
doc_type: resourcePageType
---

# customDetectionAction resource type

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Action taken on impacted entities as set in a custom detection rule.

## Properties
| Property         | Type                                                                                                                             | Description                                                                                                                                                                                                                                                                                                                                                                                                                          |
|:-----------------|:---------------------------------------------------------------------------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| actionEntities   | [microsoft.graph.security.customDetectionImpactedEntity](../resources/security-customdetectionimpactedentity.md) collection      | Entities to which the action set in the custom detection rule is applied to.                                                                                                                                                                                                                                                                                                                                                         |
| actionType       | customActionType                                                                                                                 | The actions taken on entities as set in the custom detection rule. The possible values are: `isolateDevice`, `collectInvestigationPackage`, `runAntivirusScan`, `initiateInvestigation`, `stopAndQuarantineFile`, `allowFile`, `blockFile`, `restrictAppExecution`, `markUserAsCompromised`, `moveEmailToFolder`, `deleteEmail`, `blockEmailSender`, `blockEmailUrl`, `disableUser`, `forceUserPasswordReset`, `unknownFutureValue`. |
| additionalFields | [microsoft.graph.security.customDetectionActionAdditionalFields](../resources/security-customdetectionactionadditionalfields.md) | Additional information about the custom detection rule action.                                                                                                                                                                                                                                                                                                                                                                       |

### customActionType values

| Member                        | Description                                                                                                                               |
|-------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------|
| `isolateDevice`               | Uses Microsoft Defender for Endpoint to apply full network isolation, preventing the device from connecting to any application or service |
| `collectInvestigationPackage` | Collects device information in a ZIP file                                                                                                 |
| `runAntivirusScan`            | Performs a full Microsoft Defender Antivirus scan on the device                                                                           |
| `initiateInvestigation`       | Initiates an automated investigation on the device                                                                                        |
| `stopAndQuarantineFile`       | Deletes the file from its current location and places a copy in quarantine                                                                |
| `allowFile`                   | Allows the file to run on devices controlled by Microsoft Defender for Endpoint                                                           |
| `blockFile`                   | Blocks the file from running on devices controlled by Microsoft Defender for Endpoint                                                     |
| `restrictAppExecution`        | Sets restrictions on device to allow only files that are signed with a Microsoft-issued certificate to run                                |
| `markUserAsCompromised`       | Sets the users risk level to "high" in Azure Active Directory, triggering corresponding identity protection policies                      |
| `moveEmailToFolder`           | Moves the email to a selected folder                                                                                                      |
| `deleteEmail`                 | Deletes the email message                                                                                                                 |
| `blockEmailSender`            | Blocks the email sender from sending more email to the org                                                                                |
| `blockEmailUrl`               | Blocks the URL in the email from being accessed                                                                                           |
| `disableUser`                 | Temporarily prevents a user from logging in to the on-premises network                                                                    |
| `forceUserPasswordReset`      | Prompts the user to change their password on the next sign in session                                                                     |
| `unknownFutureValue`          | unknownFutureValue for evolvable enums pattern                                                                                            |

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.customDetectionAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.customDetectionAction",
  "actionType": "String",
  "actionEntities": [
    {
      "@odata.type": "microsoft.graph.security.customDetectionImpactedEntity"
    }
  ],
  "additionalFields": {
    "@odata.type": "microsoft.graph.security.customDetectionActionAdditionalFields"
  }
}
```

