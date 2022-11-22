---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Calendar

$params = @{
	"@odata.type" = "microsoft.graph.openTypeExtension"
	ExtensionName = "Com.Contoso.Deal"
	CompanyName = "Alpine Skis"
	DealValue = 
	ExpirationDate = "2015-07-03T13:04:00.000Z"
}

New-MgBetaGroupEventExtension -GroupId $groupId -EventId $eventId -BodyParameter $params

```