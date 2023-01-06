---
title: "attackSimulationRoot resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
doc_type: resourcePageType
---

# attackSimulationRoot resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**
This is an abstract type.


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List attackSimulationRoots](../api/security-security-list-attacksimulation.md)|[attackSimulationRoot](../resources/attacksimulationroot.md) collection|Get a list of the [attackSimulationRoot](../resources/attacksimulationroot.md) objects and their properties.|
|[Create attackSimulationRoot](../api/security-security-post-attacksimulation.md)|[attackSimulationRoot](../resources/attacksimulationroot.md)|Create a new [attackSimulationRoot](../resources/attacksimulationroot.md) object.|
|[Get attackSimulationRoot](../api/attacksimulationroot-get.md)|[attackSimulationRoot](../resources/attacksimulationroot.md)|Read the properties and relationships of an [attackSimulationRoot](../resources/attacksimulationroot.md) object.|
|[Update attackSimulationRoot](../api/attacksimulationroot-update.md)|[attackSimulationRoot](../resources/attacksimulationroot.md)|Update the properties of an [attackSimulationRoot](../resources/attacksimulationroot.md) object.|
|[Delete attackSimulationRoot](../api/security-security-delete-attacksimulation.md)|None|Delete an [attackSimulationRoot](../resources/attacksimulationroot.md) object.|
|[List endUserNotifications](../api/attacksimulationroot-list-endusernotifications.md)|[endUserNotification](../resources/endusernotification.md) collection|Get the endUserNotification resources from the endUserNotifications navigation property.|
|[Create endUserNotification](../api/attacksimulationroot-post-endusernotifications.md)|[endUserNotification](../resources/endusernotification.md)|Create a new endUserNotification object.|
|[List landingPages](../api/attacksimulationroot-list-landingpages.md)|[landingPage](../resources/landingpage.md) collection|Get the landingPage resources from the landingPages navigation property.|
|[Create landingPage](../api/attacksimulationroot-post-landingpages.md)|[landingPage](../resources/landingpage.md)|Create a new landingPage object.|
|[List loginPages](../api/attacksimulationroot-list-loginpages.md)|[loginPage](../resources/loginpage.md) collection|Get the loginPage resources from the loginPages navigation property.|
|[Create loginPage](../api/attacksimulationroot-post-loginpages.md)|[loginPage](../resources/loginpage.md)|Create a new loginPage object.|
|[List trainings](../api/attacksimulationroot-list-trainings.md)|[training](../resources/training.md) collection|Get the training resources from the trainings navigation property.|
|[Create training](../api/attacksimulationroot-post-trainings.md)|[training](../resources/training.md)|Create a new training object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|endUserNotifications|[endUserNotification](../resources/endusernotification.md) collection|**TODO: Add Description**|
|landingPages|[landingPage](../resources/landingpage.md) collection|**TODO: Add Description**|
|loginPages|[loginPage](../resources/loginpage.md) collection|**TODO: Add Description**|
|operations|[attackSimulationOperation](../resources/attacksimulationoperation.md) collection|**TODO: Add Description**|
|payloads|[payload](../resources/payload.md) collection|**TODO: Add Description**|
|simulationAutomations|[simulationAutomation](../resources/simulationautomation.md) collection|**TODO: Add Description**|
|simulations|[simulation](../resources/simulation.md) collection|**TODO: Add Description**|
|trainings|[training](../resources/training.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.attackSimulationRoot",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attackSimulationRoot",
  "id": "String (identifier)"
}
```

