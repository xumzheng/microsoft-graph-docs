---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.Governance

$params = @{
	ApprovalState = "approvalState-value"
	ApproverReason = "approverReason-value"
}

Update-MgBetaPrivilegedApproval -PrivilegedApprovalId $privilegedApprovalId -BodyParameter $params

```