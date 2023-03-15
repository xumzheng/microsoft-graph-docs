---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Sites

$params = @{
	Roles = @(
		"read"
	)
}

Update-MgBetaSitePermission -SiteId $siteId -PermissionId $permissionId -BodyParameter $params

```