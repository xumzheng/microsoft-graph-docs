---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Files

$params = @{
	Name = "My Day at the Beach"
	"@microsoft.graph.conflictBehavior" = "rename"
	Bundle = @{
		Album = @{
		}
	}
	Children = @(
		@{
			Id = "1234asdf"
		}
	)
}

New-MgDriveBundle -DriveId $driveId -BodyParameter $params

```