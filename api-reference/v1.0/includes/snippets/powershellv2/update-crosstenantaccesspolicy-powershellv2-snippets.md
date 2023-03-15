---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	AllowedCloudEndpoints = @(
		"microsoftonline.us"
	)
}

Update-MgPolicyCrossTenantAccessPolicy -BodyParameter $params

```