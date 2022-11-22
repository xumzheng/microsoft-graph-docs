---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.WindowsUpdates

$params = @{
	UpdateCategory = "String"
	Assets = @(
		@{
			"@odata.type" = "#microsoft.graph.windowsUpdates.azureADDevice"
			Id = "String (identifier)"
		}
	)
}

Invoke-MgEnrollWindowsUpdatesUpdatableAsset -BodyParameter $params

```