---
title: "provisioningObjectSummary resource type"
description: "Represents an action performed by the Azure AD Provisioning service and its associated properties."
ms.localizationpriority: medium
author: "ArvindHarinder1"
ms.prod: "identity-and-access-reports"
doc_type: "resourcePageType"
---

# provisioningObjectSummary resource type

Namespace: microsoft.graph


Represents an action performed by the Azure AD Provisioning service and its associated properties. 

## Methods

| Method  | Return Type | Description |
|:-------------|:------------|:------------|
| [List provisioningObjectSummary](../api/provisioningobjectsummary-list.md) | [provisioningObjectSummary](provisioningobjectsummary.md) | Get a list of all provisioning events that occurred in your tenant. |


## Properties

| Property     | Type        | Description |
|:-------------|:------------|:------------|
|activityDateTime|DateTimeOffset|The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`|
|changeId|String|Unique ID of this change in this cycle.|
|cycleId|String|Unique ID per job iteration.|
|durationInMilliseconds|Int32|Indicates how long this provisioning action took to finish. Measured in milliseconds.|
|id|String| Indicates the unique ID for the activity. This is a read-only GUID.|
|initiatedBy|[initiator](initiator.md)|Details of who initiated this provisioning.|
|jobId|String|The unique ID for the whole provisioning job.|
|modifiedProperties|[modifiedProperty](modifiedproperty.md) collection|Details of each property that was modified in this provisioning action on this object.|
|provisioningAction|provisioningAction|Indicates the activity name or the operation name. Possible values are: `create`, `update`, `delete`, `stageddelete`, `disable`, `other` and `unknownFutureValue`. For a list of activities logged, refer to Azure AD activity list.|
|provisioningStatusInfo|[provisioningStatusInfo](provisioningstatusinfo.md)|Details of provisioning status.|
|provisioningSteps|[provisioningStep](provisioningstep.md) collection|Details of each step in provisioning.|
|servicePrincipal|[servicePrincipal](provisioningserviceprincipal.md) collection|Represents the service principal used for provisioning.|
|sourceIdentity|[provisionedIdentity](provisionedidentity.md)|Details of source object being provisioned.|
|sourceSystem|[provisioningSystem](provisioningsystem.md)|Details of source system of the object being provisioned.|
|targetIdentity|[provisionedIdentity](provisionedidentity.md)|Details of target object being provisioned.|
|targetSystem|[provisioningSystem](provisioningsystem.md)|Details of target system of the object being provisioned.|
|tenantId|String|Unique Azure AD tenant ID.|

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningObjectSummary",
  "keyProperty": "id"
}-->

```json
{
  "provisioningAction":  "String",
  "activityDateTime": "String (timestamp)",
  "changeId": "String",
  "cycleId": "String",
  "durationInMilliseconds": 1024,
  "id": "String (identifier)",
  "initiatedBy": {"@odata.type": "microsoft.graph.initiator"},
  "jobId": "String",
  "modifiedProperties": [{"@odata.type": "microsoft.graph.modifiedProperty"}],
  "provisioningSteps": [{"@odata.type": "microsoft.graph.provisioningStep"}],
  "servicePrincipal": [{"@odata.type": "microsoft.graph.provisioningServicePrincipal"}],
  "sourceIdentity": {"@odata.type": "microsoft.graph.provisionedIdentity"},
  "sourceSystem": {"@odata.type": "microsoft.graph.provisioningSystem"},
  "provisioningStatusInfo": {"@odata.type": "microsoft.graph.provisioningStatusInfo"},
  "targetIdentity": {"@odata.type": "microsoft.graph.provisionedIdentity"},
  "targetSystem": {"@odata.type": "microsoft.graph.provisioningSystem"},
  "tenantId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningObjectSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


