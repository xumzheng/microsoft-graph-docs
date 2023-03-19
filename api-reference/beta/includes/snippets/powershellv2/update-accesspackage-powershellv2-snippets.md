---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.Governance

$params = @{
	DisplayName = "Access Package New Name"
}

Update-MgBetaEntitlementManagementAccessPackage -AccessPackageId $accessPackageId -BodyParameter $params

```