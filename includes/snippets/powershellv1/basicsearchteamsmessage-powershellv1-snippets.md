---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Search

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

Invoke-MgQuerySearch -BodyParameter $params

```