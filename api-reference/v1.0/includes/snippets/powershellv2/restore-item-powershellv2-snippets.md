---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Files

$params = @{
	parentReference = @{
		id = "String"
	}
	name = "String"
}

Restore-MgBetaDrivesItem -DriveId $driveId -DriveItemId $driveItemId -BodyParameter $params

```