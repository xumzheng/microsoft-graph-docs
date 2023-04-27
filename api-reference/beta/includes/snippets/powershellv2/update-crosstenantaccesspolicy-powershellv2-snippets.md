---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	allowedCloudEndpoints = @(
		"microsoftonline.us"
		"partner.microsoftonline.cn"
	)
}

Update-MgBetaPolicyCrossTenantAccessPolicy -BodyParameter $params

```