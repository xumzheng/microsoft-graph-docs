---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
	DisplayName = "Catalog One"
}

Update-MgEntitlementManagementAccessPackageCatalog -AccessPackageCatalogId $accessPackageCatalogId -BodyParameter $params

```