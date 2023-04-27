---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
	displayName = "Catalog One"
}

Update-MgEntitlementManagementCatalog -AccessPackageCatalogId $accessPackageCatalogId -BodyParameter $params

```