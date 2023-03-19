---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Search

$params = @{
	Requests = @(
		@{
			EntityTypes = @(
				"chatMessage"
			)
			Query = @{
				QueryString = "test"
			}
			From = 0
			Size = 25
		}
	)
}

Invoke-MgBetaQuerySearch -BodyParameter $params

```