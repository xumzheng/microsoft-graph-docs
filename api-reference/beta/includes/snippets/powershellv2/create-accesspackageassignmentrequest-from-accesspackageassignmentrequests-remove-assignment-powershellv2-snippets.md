---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.Governance

$params = @{
	RequestType = "AdminRemove"
	AccessPackageAssignment = @{
		Id = "a6bb6942-3ae1-4259-9908-0133aaee9377"
	}
}

New-MgBetaEntitlementManagementAccessPackageAssignmentRequest -BodyParameter $params

```