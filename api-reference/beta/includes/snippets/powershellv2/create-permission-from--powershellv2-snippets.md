---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Sites

$params = @{
	Roles = @(
		"write"
	)
	GrantedToIdentities = @(
		@{
			Application = @{
				Id = "89ea5c94-7736-4e25-95ad-3fa95f62b66e"
				DisplayName = "Contoso Time Manager App"
			}
		}
	)
}

New-MgBetaSitePermission -SiteId $siteId -BodyParameter $params

```