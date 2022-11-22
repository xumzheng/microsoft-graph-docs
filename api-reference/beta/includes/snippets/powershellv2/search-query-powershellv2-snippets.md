---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Search

$params = @{
	Requests = @(
		@{
			EntityTypes = @(
				"externalItem"
			)
			ContentSources = @(
				"/external/connections/connectionfriendlyname"
			)
			Query = @{
				QueryString = "contoso product"
			}
			From = 0
			Size = 25
			Fields = @(
				"title"
				"description"
			)
		}
	)
}

Invoke-MgBetaQuerySearch -BodyParameter $params

```