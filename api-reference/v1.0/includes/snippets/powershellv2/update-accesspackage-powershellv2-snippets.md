---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
	DisplayName = "Access Package New Name"
}

Update-MgEntitlementManagementAccessPackage -AccessPackageId $accessPackageId -BodyParameter $params

```