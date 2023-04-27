---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
	id = "request-id"
	requestStatus = "cancelled"
}

Stop-MgEntitlementManagementAccessPackageAssignmentRequest -AccessPackageAssignmentRequestId $accessPackageAssignmentRequestId -BodyParameter $params

```