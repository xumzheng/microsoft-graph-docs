---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.Governance

$params = @{
	CatalogId = "aa2f6514-3232-46e7-a08a-2411ad8d7128"
	DisplayName = "sales reps"
	Description = "outside sales representatives"
}

New-MgBetaEntitlementManagementAccessPackage -BodyParameter $params

```