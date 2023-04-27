---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	displayName = "Custom permission grant policy"
}

Update-MgPolicyPermissionGrantPolicy -PermissionGrantPolicyId $permissionGrantPolicyId -BodyParameter $params

```