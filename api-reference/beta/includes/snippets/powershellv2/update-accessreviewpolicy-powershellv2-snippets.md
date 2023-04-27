---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	isGroupOwnerManagementEnabled = $true
}

Update-MgBetaPolicyAccessReviewPolicy -BodyParameter $params

```