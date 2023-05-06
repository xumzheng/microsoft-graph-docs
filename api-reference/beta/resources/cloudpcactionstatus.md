---
title: "cloudPcActionStatus resource type"
description: "Cloud managed virtual desktops."
author: "Aria Zhang"
ms.localizationpriority: medium
ms.prod: "cloud-pc"
doc_type: resourcePageType
---

# cloudPcActionStatus resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents a cloud-managed virtual desktop device action status.

## Methods

|Method|Return type|Description|
|:---|:---|:---|
|[List cloudPcActionStatuses](../api/virtualendpoint-list-cloudpcactionstatuses.md)|[cloudPcActionStatus](../resources/cloudpcactionstatus.md) collection|List properties and relationships of the [cloudPcActionStatus](../resources/cloudpc.md) objects.|
|[Get cloudPcActionStatus](../api/cloudpcactionstatus-get.md)|[cloudPcActionStatus](../resources/cloudpcactionstatus.md)|Read the properties and relationships of a [cloudPcActionStatus](../resources/cloudpcactionstatus.md) object.|
## Properties

|Property|Type|Description|
|:---|:---|:---|
|id|String|The unique identifier for the Cloud PC action status. Read-only.|
|cloudPcId|String|The unique identifier for the Cloud PC. Read-only.|
|cloudPcDeviceDisplayName|String|Name of the Cloud PC.|
|initiatedByUserPrincipalName|String|The user principal name (UPN) of the ITPro (IT admin) who initiated the request.|
|deviceOwnerUserPrincipalName|String|The user principal name (UPN) of the user assigned to the Cloud PC.|
|bulkActionId|String|Bulk action id, will be null when it's single triggered.|
|bulkActionDisplayName|String|Customized bulk action name, will be null if it's single trigger.|
|action|[cloudPcRemoteActionName](#cloudpcremoteactionname-values)|The action name. Cloud PC related possible values are: `unknown`,`restart`,`rename`,`resize`,`restore`,`reprovision`,`changeUserAccountType`,`troubleshoot`,`placeUnderReview`, `powerOn`, `powerOff`.|
|actionState|[actionState](#actionstate-values)|State of the action. Possible values are: `None`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`. Read-only.|
|requestDateTime|DateTimeOffset|Time when the action was issued.The timestamp is shown in ISO 8601 format and Coordinated Universal Time (UTC). For example, midnight UTC on Jan 1, 2014 appears as '2014-01-01T00:00:00Z'.|
|lastUpdatedDateTime|DateTimeOffset|The last update time of the Cloud PC remote action. The timestamp is shown in ISO 8601 format and Coordinated Universal Time (UTC). For example, midnight UTC on Jan 1, 2014 appears as '2014-01-01T00:00:00Z'.|
|statusDetails|[cloudPcStatusDetails](../resources/cloudpcstatusdetails.md)|The details of the remote action status. Example: `{ "code": "internalServerError", "message": "There was an error during the Cloud PC upgrade. Please contact support.", "additionalInformation": null }`.|

### cloudPcRemoteActionName values

|Member|Description|
|:---|:---|
|unknown|Indicates the remote action name as `unknown` when the remote action name is unknown and not in the list. Default.|
|restart|Indicates the remote action name as `restart`. Use this action to restart a Cloud PC.|
|rename|Indicates the remote action name as `rename`. Use this action to update the display name of a Cloud PC.|
|resize|Indicates the remote action name as `resize`. Use this action to upgrade or downgrade a Cloud PC by changing its service plan. For example, from 2 vCPU to 4 vCPU.|
|restore|Indicates the remote action name as `restore`. Use this action to restore a Cloud PC to a previous state from a snapshot.|
|reprovision|Indicates the remote action name as `reprovision`. Use this action to re-create a Cloud PC by a given Cloud PC ID if any unresolvable issue occurs.|
|changeUserAccountType|Indicates the remote action name as `changeUserAccountType`. Use this action to change the account type of the user of a Cloud PC. For example, from a standard user to an administrator.|
|troubleshoot|Indicates the remote action name as `troubleshoot`. Use this action to check the health status of the Cloud PC and the session host.|
|placeUnderReview|Indicates the remote action name as `placeUnderReview`. Use this action to set the Cloud PC to review state or set it back, when the Cloud PC is considered suspicious.|
|powerOn|Indicates the remote action name as `powerOn`. Use this action to power on the Cloud PC.|
|powerOff|Indicates the remote action name as `powerOff`. Use this action to power off the Cloud PC.|
|unknownFutureValue|Evolvable enumeration sentinel value. Do not use.|

### actionState values

|Member|Description|
|:---|:---|
|none|Not a valid action state.|
|pending|Action is pending.|
|canceled|Action has been cancelled.|
|active|Action is active.|
|done|Action completed without errors.|
|failed|Action failed.|
|notSupported|Action is not supported.|

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcActionStatus",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcActionStatus",
  "id": "662009bc-7732-4f6f-8726-25883518b33e",
  "cloudPcDeviceDisplayName": "CloudPC-Connie",
  "bulkActionId": "bdc8e6dd-0455-4412-83d9-c818664fe1f1",
  "bulkActionDisplayName": "Resize to 64GB RAM - John",
  "cloudPcId": "bdc8e6dd-0455-4412-83d9-c818664fe1f1",
  "initiatedByUserPrincipalName": "john@cpccustomer001.onmicrosoft.com",
  "deviceOwnerUserPrincipalName": "connie@cpccustomer001.onmicrosoft.com",
  "action": "Resize",
  "actionState": "failed",
  "requestDateTime": "2020-07-23T10:10:57Z",
  "lastUpdatedDateTime": "2020-07-23T10:29:57Z"
}
```
