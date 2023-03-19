---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
	DisplayName = "sales"
	Description = "for employees working with sales and outside sales partners"
	State = "published"
	IsExternallyVisible = $true
}

New-MgEntitlementManagementCatalog -BodyParameter $params

```