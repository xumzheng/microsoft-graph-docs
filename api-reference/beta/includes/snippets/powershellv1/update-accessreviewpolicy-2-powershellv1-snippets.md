---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
	IsGroupOwnerManagementEnabled = $true
}

Update-MgIdentityGovernanceAccessReviewPolicy -BodyParameter $params

```