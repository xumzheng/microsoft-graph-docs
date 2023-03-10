---
title: "attackSimulationRoot resource type"
description: "Represents an abstract type that provides the ability to launch a realistic phishing attack that organizations can learn from."
author: "stuartcl"
ms.localizationpriority: medium
ms.prod: "security"
doc_type: resourcePageType
---

# attackSimulationRoot resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List simulations](../api/attacksimulationroot-list-simulations.md)|[simulation](../resources/simulation.md) collection|Get a list of attack simulation campaigns for a tenant.|
|[Get simulations](../api/simulation-get.md)|[simulation](../resources/simulation.md) |Get an attack simulation campaigns for a tenant.|
|[Create simulations](../api/attacksimulationroot-post-simulation.md)|[simulation](../resources/simulation.md)|Create a new attack simulation campaigns for a tenant.|
|[Update simulations](../api/simulation-update.md)|[simulation](../resources/simulation.md)|Update a attack simulation campaigns for a tenant.|
|[Delete simulations](../api/simulation-delete.md)|[simulation](../resources/simulation.md)|Delete a attack simulation campaigns for a tenant.|
|[List simulationAutomations](../api/attacksimulationroot-list-simulationautomations.md)|[simulationAutomation](../resources/simulationautomation.md) collection|Get a list of attack simulation automations for a tenant.|
|[Get simulationAutomations](../api/simulationautomation-get.md)|[simulationAutomation](../resources/simulationautomation.md) |Get an attack simulation automations for a tenant.|
|[List payloads](../api/attacksimulationroot-list-payloads.md)|[payload](../resources/payload.md) collection|Get the payload resources from the payloads navigation property.|
|[Get payloads](../api/payload-get.md)|[payload](../resources/payload.md)|Get the payload resource from the payloads navigation property.|
|[Get attackSimulationOperation](../api/attacksimulationoperation-get.md)|[attackSimulationOperation](../resources/attacksimulationoperation.md)|Get an attack simulation campaign operation for a tracking ID.|
|[List endUserNotifications](../api/attacksimulationroot-list-endusernotifications.md)|[endUserNotification](../resources/endusernotification.md) collection|Get the endUserNotification resources from the endUserNotifications navigation property.|
|[Get endUserNotifications](../api/attacksimulationroot-get-endUserNotifications.md)|[endUserNotification](../resources/endUserNotification.md)|Get the endUserNotification resources from the endUserNotifications navigation property.|
|[List landingPages](../api/attacksimulationroot-list-landingpages.md)|[landingPage](../resources/landingpage.md) collection|Get the landingPage resources from the landingPages navigation property.|
|[Get landingPages](../api/attacksimulationroot-list-landingpages.md)|[landingPage](../resources/landingpage.md) |Get the landingPage resources from the landingPages navigation property.|
|[List loginPages](../api/attacksimulationroot-list-loginpages.md)|[loginPage](../resources/loginpage.md) collection|Get the loginPage resources from the loginPages navigation property.|
|[Get loginPages](../api/attacksimulationroot-list-loginpages.md)|[loginPage](../resources/loginpage.md)|Get the loginPage resources from the loginPages navigation property.|
|[List trainings](../api/attacksimulationroot-list-trainings.md)|[training](../resources/training.md) collection|Get the training resources from the trainings navigation property.|

## Properties
None.

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|operations|[attackSimulationOperation](../resources/attacksimulationoperation.md) collection|Represents an attack simulation training operation.|
|payloads|[payload](../resources/payload.md) collection|Represents an attack simulation training campaign payload in a tenant.|
|simulationAutomations|[simulationAutomation](../resources/simulationautomation.md) collection|Represents simulation automation created to run on a tenant.|
|simulations|[simulation](../resources/simulation.md) collection|Represents an attack simulation training campaign in a tenant.|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.attackSimulationRoot",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attackSimulationRoot"
}
```
