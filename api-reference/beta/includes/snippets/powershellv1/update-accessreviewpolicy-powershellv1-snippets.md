---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	IsGroupOwnerManagementEnabled = $true
}

Update-MgPolicyAccessReviewPolicy -BodyParameter $params

```