---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
	reviewResult = "Approve"
	justification = "OK"
}

Update-MgEntitlementManagementAccessPackageAssignmentApprovalStage -ApprovalId $approvalId -ApprovalStageId $approvalStageId -BodyParameter $params

```