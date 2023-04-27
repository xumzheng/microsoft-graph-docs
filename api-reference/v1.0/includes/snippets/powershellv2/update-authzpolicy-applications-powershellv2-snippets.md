---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	defaultUserRolePermissions = @{
		allowedToCreateApps = $false
	}
}

Update-MgPolicyAuthorizationPolicy -BodyParameter $params

```