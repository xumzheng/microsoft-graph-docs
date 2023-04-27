---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Calendar

$params = @{
	"@odata.type" = "microsoft.graph.room"
	nickname = "Conf Room"
	building = "1"
	label = "100"
	capacity = 50
	isWheelChairAccessible = $false
}

Update-MgBetaPlace -PlaceId $placeId -BodyParameter $params

```