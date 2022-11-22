---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.Governance

$params = @{
	DisplayName = "sales"
	Description = "for employees working with sales and outside sales partners"
	IsExternallyVisible = $true
}

New-MgBetaEntitlementManagementAccessPackageCatalog -BodyParameter $params

```