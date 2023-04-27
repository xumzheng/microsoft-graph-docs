---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	allowedToUseSSPR = $true
}

Update-MgPolicyAuthorizationPolicy -BodyParameter $params

```