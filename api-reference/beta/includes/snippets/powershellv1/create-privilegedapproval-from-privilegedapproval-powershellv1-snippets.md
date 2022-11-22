---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
	UserId = "userId-value"
	RoleId = "roleId-value"
	ApprovalType = "approvalType-value"
	ApprovalState = "approvalState-value"
	ApprovalDuration = "datetime-value"
}

New-MgPrivilegedApproval -BodyParameter $params

```