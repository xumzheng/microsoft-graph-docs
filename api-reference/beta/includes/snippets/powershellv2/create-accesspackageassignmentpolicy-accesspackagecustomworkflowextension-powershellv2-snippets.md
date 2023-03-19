---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.Governance

$params = @{
	DisplayName = "extension-policy"
	Description = "test"
	AccessPackageId = "ba5807c7-2aa9-4c8a-907e-4a17ee587500"
	CanExtend = $false
	RequestApprovalSettings = $null
	RequestorSettings = @{
		AcceptRequests = $true
		ScopeType = "AllExistingDirectorySubjects"
		AllowedRequestors = @(
		)
		IsOnBehalfAllowed = $false
	}
	AccessReviewSettings = $null
	Questions = @(
	)
	CustomExtensionStageSettings = @(
	)
}

New-MgBetaEntitlementManagementAccessPackageAssignmentPolicy -BodyParameter $params

```