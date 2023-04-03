---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Files

$params = @{
	Name = "Just some files"
	"@microsoft.graph.conflictBehavior" = "rename"
	Bundle = @{
	}
	Children = @(
		@{
			Id = "1234asdf"
		}
		@{
			Id = "1234qwerty"
		}
	)
}

New-MgDriveBundle -DriveId $driveId -BodyParameter $params

```