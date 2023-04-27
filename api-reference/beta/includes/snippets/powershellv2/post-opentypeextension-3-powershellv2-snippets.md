---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Calendar

$params = @{
	"@odata.type" = "microsoft.graph.openTypeExtension"
	extensionName = "Com.Contoso.Deal"
	companyName = "Alpine Skis"
	dealValue = 1010100
	expirationDate = "2015-07-03T13:04:00.000Z"
}

New-MgBetaGroupEventExtension -GroupId $groupId -EventId $eventId -BodyParameter $params

```