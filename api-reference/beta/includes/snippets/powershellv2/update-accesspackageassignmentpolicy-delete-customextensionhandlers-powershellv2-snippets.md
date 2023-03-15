---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.Governance

$params = @{
	Id = "4540a08f-8ab5-43f6-a923-015275799197"
	DisplayName = "policy with custom access package workflow extension"
	Description = "Run specified custom access package workflow extension at different stages."
	AccessPackageId = "ba5807c7-2aa9-4c8a-907e-4a17ee587500"
	RequestApprovalSettings = $null
	RequestorSettings = @{
		AcceptRequests = $true
		ScopeType = "AllExistingDirectorySubjects"
		AllowedRequestors = @(
		)
	}
	AccessReviewSettings = $null
	CustomExtensionHandlers = @(
	)
}

Set-MgBetaEntitlementManagementAccessPackageAssignmentPolicy -AccessPackageAssignmentPolicyId $accessPackageAssignmentPolicyId -BodyParameter $params

```