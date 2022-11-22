---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
	DisplayName = "sales"
	Description = "for employees working with sales and outside sales partners"
	IsExternallyVisible = $true
}

New-MgEntitlementManagementAccessPackageCatalog -BodyParameter $params

```