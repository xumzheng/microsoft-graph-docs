---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Groups

$params = @{
	"Members@odata.bind" = @(
		"https://graph.microsoft.com/v1.0/directoryObjects/{id}"
		"https://graph.microsoft.com/v1.0/directoryObjects/{id}"
		"https://graph.microsoft.com/v1.0/directoryObjects/{id}"
	)
}

Update-MgGroup -GroupId $groupId -BodyParameter $params

```